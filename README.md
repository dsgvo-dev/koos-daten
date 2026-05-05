# KOOS — Kern-Organisations-Operations-System

Ein dateibasiertes Wissensystem für Kommunalverwaltungen.

> **Datenformat-Repo.** Die Referenzimplementierung (Server + Browser-Oberfläche) liegt unter
> [github.com/dsgvo-dev/koos-server](https://github.com/dsgvo-dev/koos-server).

---

## Was steckt im Namen?

**K** steht für *Kern* — im doppelten Sinne:

Als **Grundlage und Wesentliches**: KOOS ist kein Programm, das man installiert, sondern das Kernstück eines Organisations-Wissensystems — die Konvention, nach der Informationen gespeichert, verknüpft und versioniert werden.

Als **Kernel im Unix-Sinne**: Genau wie der Linux-Kernel festlegt, wie Prozesse mit Ressourcen interagieren, legt KOOS fest, wie Verwaltungsprozesse mit Daten, Organisationseinheiten und Regelungen zusammenhängen. Der Resolver ist das `/proc`-Dateisystem von KOOS — er berechnet Rückverweise und ID-Tabellen zur Laufzeit, ohne selbst Daten zu speichern.

**OOS** steht für *Organisations-Operations-System* — das Betriebssystem für Organisationswissen.

---

## Kurzübersicht

KOOS besteht aus:

- **Textdateien** (`orga.yaml`, `prozesse/*.md`, `daten/*.md`, `regelungen/*.md`) als einzige Quelle der Wahrheit
- **`koos.yaml`** als zentrale Konfiguration (Organisation, Nutzer, Vokabular)
- Einem **Resolver** — zur Laufzeit implementiert in einem kompatiblen Viewer — der IDs auflöst und Rückverweise berechnet

```
koos-daten/
  orga.yaml          ← Organisationsstruktur
  koos.yaml          ← Konfiguration
  prozesse/*.md      ← Prozesse
  daten/*.md         ← Datenarten
  regelungen/*.md    ← Regelungen
```

Alle Dateien sind im Texteditor pflegbar, in Git versioniert und von jedem kompatiblen Viewer lesbar.

---

## Inhalt

- [Leitgedanken: UNIX, NixOS, Git, ADR](#leitgedanken-unix-nixos-git-adr)
- [Die vier Informationsdimensionen](#die-vier-informationsdimensionen)
- [Grundprinzip: Stabile IDs](#grundprinzip-stabile-ids)
- [Verlinkung: Wie Entitäten zusammenhängen](#verlinkung-wie-entitäten-zusammenhängen)
- [Dateiformate](#dateiformate)
- [Vokabular — kontrollierte Wertelisten](#vokabular--kontrollierte-wertelisten)
- [Rollenmodell in orga.yaml](#rollenmodell-in-orgayaml)
- [Git als unveränderlicher Speicher](#git-als-unveränderlicher-speicher)
- [Regelungen als ADR](#regelungen-als-adr)
- [Zwei Varianten](#zwei-varianten)
- [Referenzielle Integrität](#referenzielle-integrität)
- [Tradeoffs](#tradeoffs)
- [Entwicklungsstand](#entwicklungsstand)

---

## Leitgedanken: UNIX, NixOS, Git, ADR

KOOS lehnt sich bewusst an vier Grundkonzeptionen an, die sich in der Softwarewelt über Jahrzehnte bewährt haben:

| Vorbild | Konzept | KOOS-Entsprechung |
|---|---|---|
| **Unix** | Everything is a File; Prozesse als zentrale Entitäten | Alle Entitäten sind Dateien; Prozesse verbinden OE, Daten, Regelungen |
| **NixOS** | Deklarative Konfiguration; Reproducibility; Generationen | `koos.yaml`; Clone = vollständige Instanz; Git-Tags als Generationen |
| **Git** | Unveränderliche Geschichte; Content-Addressing | Versionshistorie aller Änderungen; Freigaben als Tags; Gabeln als Instanzen |
| **ADR** | Architecture Decision Records: Entscheidungen mit Kontext | Regelungen mit Begründung, Alternativen, Datum |

### Everything is a File (UNIX)

KOOS ist bewusst im Geist des Unix-Prinzips gebaut:

- **Prozesse** sind die primären Entitäten — sie binden alle anderen Dimensionen zusammen, wie Betriebssystemprozesse Ressourcen binden.
- **Datenarten** sind Ressourcen, auf die Prozesse zugreifen — wie Dateien, die gelesen oder geschrieben werden.
- **OE** sind Eigentümer und Zuständige — wie Benutzer und Gruppen in Unix.
- **Regelungen** sind Constraints — wie Zugriffsrechte und Kernel-Policies.

Der **Resolver** (implementiert in einem kompatiblen Viewer) entspricht dem `/proc`-Dateisystem in Linux: Er berechnet seinen Inhalt — die ID→Name-Tabelle, Rückverweise — bei jedem Zugriff neu aus dem aktuellen Systemzustand. Er speichert nichts selbst.

Die **stabile ID** entspricht dem Inode: Der Dateiname (Anzeigename) kann sich ändern, die ID bleibt konstant. Verknüpfungen über IDs brechen nie — egal wie oft die Organisation umbenannt wird.

### Deklarative Konfiguration (NixOS)

In NixOS beschreibt `configuration.nix` das gesamte System deklarativ. Ein Rebuild liest die Konfiguration und leitet daraus den gewünschten Systemzustand ab. Ältere Generationen bleiben im Nix Store erhalten.

KOOS überträgt dieses Prinzip auf Organisationswissen:

| NixOS | KOOS |
|---|---|
| `configuration.nix` | `koos.yaml` (Root-Konfiguration) |
| Module (`services.nginx`, `users.*`) | Dimensionen: OE, Prozesse, Daten, Regelungen |
| Derivations → Systemzustand | Resolver → ID→Name-Tabelle, Querverweise |
| Nix Store (unveränderlich, inhaltsadressiert) | Git-Repository |
| Generationen / `nixos-rebuild switch` | Git-Tags / manuelle Freigaben |

Das bedeutet konkret:

- **Eine Quelle der Wahrheit pro Entität.** Die OE-Hierarchie lebt in `orga.yaml`, Prozesse in `prozesse/*.md`, Datenarten in `daten/*.md`. Nirgendwo sonst.
- **Umbenennung = eine Zeile.** Weil Verknüpfungen auf stabile IDs zeigen, nicht auf Namen.
- **Der Resolver rechnet, nicht die Pflegeperson.** Welche Prozesse nutzen eine Datenart? Das berechnet das System zur Anzeigezeit — aus denselben Dateien, die ohnehin existieren.

---

## Die vier Informationsdimensionen

Organisationswissen hat vier Grunddimensionen. Alle vier sind miteinander verknüpft, aber jede lebt in ihrer eigenen Datei oder ihrem eigenen Ordner:

```
         Regelungen
      (Was gilt?)
  Gesetze, Dienstanweisungen
           ↕
OE ──── Prozess ──── Daten
(Wer?) (Was?)       (Womit?)
```

| Dimension | Frage | Datei / Ordner | ID-Präfix |
|---|---|---|---|
| **OE** – Organisationseinheiten | Wer ist zuständig? | `orga.yaml` | `oe-` |
| **Prozesse** | Was passiert, in welchen Schritten? | `prozesse/*.md` | `proc-` |
| **Daten** | Was wird verarbeitet, wie lange, nach welchem Recht? | `daten/*.md` | `dstore-` |
| **Regelungen** | Was ist vorgegeben (Gesetz, Dienstanweisung)? | `regelungen/*.md` | `reg-` |

**Prozesse stehen im Zentrum:** Jeder Prozess nennt seine zuständige OE, die beteiligten Einheiten, die verarbeiteten Datenarten und die geltenden Regelungen — alles als stabile IDs.

### Datenmodell: Drei Arten von Daten im Prozess

Nach BPMN 2.0 (ISO 19510) unterscheidet KOOS drei Typen:

| Typ | Bedeutung | Im Prozess |
|---|---|---|
| **Input** | Was der Prozess als Eingang braucht | `daten.input:` — Freitext |
| **Output** | Was der Prozess erzeugt | `daten.output:` — Freitext |
| **Datenspeicher** | Persistente Bestände, die gelesen/geschrieben werden | `daten.datenspeicher:` — Referenz auf `dstore-*` |

---

## Grundprinzip: Stabile IDs

Jede Entität hat zwei Felder:

```yaml
id:   dstore-personalakte      # stabile Kennung — NIEMALS ändern
name: Personalakte             # Anzeigename — jederzeit in dieser einen Datei änderbar
```

**Der Dateiname ist die ID.** `daten/dstore-personalakte.md` trägt automatisch die ID `dstore-personalakte`. Kein separates Mapping-File notwendig.

**Verknüpfungen zeigen immer auf die ID:**

```yaml
# In prozesse/proc-onboarding.md:
zustaendigeEinheit: oe-fb1-personal
daten:
  datenspeicher:
    - id: dstore-personalakte
    - id: dstore-it-berechtigungsantrag
```

**Der Resolver** baut beim Laden eine `ID → Anzeigename`-Tabelle aus allen Frontmattern auf und löst IDs beim Rendern auf:

```
oe-fb1-personal       →  "1.1 – Personal und Organisation"
dstore-personalakte   →  "Personalakte"
proc-onboarding       →  "Onboarding neuer Mitarbeiter/innen"
```

### ID-Konvention

| Typ | Präfix | Beispiel |
|---|---|---|
| Prozess | `proc-` | `proc-baugenehmigung-beantragen` |
| Datenart | `dstore-` | `dstore-personalakte` |
| Regelung | `reg-` | `reg-adga-001` |
| Organisationseinheit | `oe-` | `oe-amt-63` |

ID-Bildungsregel: `präfix` + kebab-case des Anzeigenamens (Umlaute ausschreiben: ä→ae, ö→oe, ü→ue, ß→ss, Leerzeichen→-).

### Häufige Änderungen — Aufwand

| Änderung | Anpassung |
|---|---|
| OE umbenennen | 1 Zeile in `orga.yaml` (`name:`) |
| Datenart umbenennen | 1 Zeile in `daten/dstore-xxx.md` (`name:`) |
| OE verschieben (Reorganisation) | 1 Zeile in `orga.yaml` (`parent:` ändern); Prozesse unberührt |
| Schutzstufe / Schutzbedarf ändern | 1 Feld in `daten/dstore-xxx.md` |
| Neuen Prozess anlegen | Neue Datei in `prozesse/` |
| Neue Verknüpfung im Prozess | ID der Zieldatei eintragen |

---

## Verlinkung: Wie Entitäten zusammenhängen

### Einmalige Referenz, berechnete Rückrichtung

KOOS speichert jede Beziehung genau einmal — am Prozess. Weder `orga.yaml` noch `daten/*.md` enthalten Listen von Prozessen. Alle Rückrichtungen berechnet der Resolver zur Laufzeit.

```
orga.yaml        →  keine Prozessliste
daten/*.md       →  keine Prozessliste
prozesse/*.md    →  zustaendigeEinheit: oe-fb1-personal
                 →  beteiligte[].einheit: oe-fb1-it
                 →  daten.datenspeicher: [dstore-personalakte, ...]
Resolver         →  prozesseFuerOE(oeId)   → zuständige + beteiligte Prozesse
                 →  filter(datenspeicher)  → verwendende Prozesse für eine Datenart
```

Das bedeutet in der Praxis: Ein neuer Prozess wird nur in seiner eigenen Datei gepflegt. OE-Dateien und Daten-Dateien bleiben dabei unberührt.

### Verlinkung: Prozesse ↔ OE

```yaml
id: proc-onboarding
zustaendigeEinheit: oe-fb1-personal      # Primär verantwortliche OE
zustaendigeRolle: Abteilungsleitung Personal

beteiligte:
  - einheit: oe-fb1-it
    aufgabe: Einrichtung IT-Arbeitsplatz, Vergabe Zugriffsrechte
```

| Feld | Bedeutung |
|---|---|
| `zustaendigeEinheit` | OE „besitzt" und steuert den Prozess |
| `beteiligte[].einheit` | OE führt einen Teilschritt aus |

### Verlinkung: Prozesse ↔ Daten

Der Prozess nennt die Datenarten, die er verarbeitet. Die Datenart-Datei enthält keine Gegenliste. Im Daten-Detail erscheint automatisch ein Abschnitt **Verwendet in**, der alle referenzierenden Prozesse auflistet.

### Überblick: Wer referenziert wen?

| Von | Nach | Feld | Rückrichtung |
|---|---|---|---|
| Prozess | OE (zuständig) | `zustaendigeEinheit` | `prozesseFuerOE(oeId).zuständig` |
| Prozess | OE (beteiligt) | `beteiligte[].einheit` | `prozesseFuerOE(oeId).beteiligt` |
| Prozess | Datenspeicher | `daten.datenspeicher[].id` | `filter(p ⇒ p.daten.datenspeicher.includes(id))` |

Die Pfeile zeigen immer in dieselbe Richtung: **Prozess → alles andere.** Die umgekehrten Anzeigen sind ausschließlich berechnete Rückverweise — keine gepflegten Felder.

---

## Dateiformate

### Organisationsstruktur (`orga.yaml`)

Die Datei `orga.yaml` enthält die gesamte Organisationshierarchie als **flache Liste** von Einheiten mit `parent`-Verweisen. Reorganisation = `parent:`-Wert ändern, fertig.

```yaml
name: Gemeindeverwaltung Musterstadt

einheiten:
  - id: oe-hvb
    name: Bürgermeister/in (HVB)
    parent: ~                      # ~ = Wurzelknoten
    rollen:
      - Bürgermeister/in

  - id: oe-stabsstelle
    name: Stabsstelle Organisation
    parent: oe-hvb
    rollen:
      - Leitung Stabsstelle
    sonderfunktionen:
      - Datenschutzbeauftragte/r
    hinweis: >
      Zuständig für KOOS-Pflege und Prozessmanagement.
```

| Feld | Pflicht | Beschreibung |
|---|---|---|
| `id` | ✓ | Stabile ID mit Präfix `oe-` — niemals nachträglich ändern |
| `name` | ✓ | Anzeigename — jederzeit in dieser Datei änderbar |
| `parent` | ✓ | ID der übergeordneten OE; `~` für Wurzelknoten |
| `rollen` | — | OE-spezifische Rollen (Freitext-Liste) |
| `sonderfunktionen` | — | Organisationsweit wirksame Funktionen |
| `hinweis` | — | Freitext-Anmerkung |

---

### Datenarten (`daten/dstore-*.md`)

```markdown
---
id: dstore-personalakte
name: Personalakte
datenkategorie: Personaldaten
zuständige-einheit: oe-fb1-personal

klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
    - BDSG §26
    - NKomVG §86
    - DSGVO Art. 88
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Ausscheiden

letzte-aktualisierung: 2026-04-01
---

# Personalakte

## Definition
...
```

| Feld | Pflicht | Beschreibung |
|---|---|---|
| `id` | ✓ | Stabile ID mit Präfix `dstore-` |
| `name` | ✓ | Anzeigename |
| `datenkategorie` | ✓ | Kontrolliertes Vokabular aus `koos.yaml` |
| `klassifizierung.schutzstufe` | ✓ | Datenschutzklassifizierung A–E |
| `klassifizierung.schutzbedarf` | ✓ | BSI IT-Grundschutz: normal / hoch / sehr hoch |
| `klassifizierung.vertraulichkeit` | ✓ | Zugangskontrolle nach ISO 27001 |
| `klassifizierung.rechtsgrundlagen` | — | Anwendbare Rechtsgrundlagen |
| `klassifizierung.aufbewahrung.frist` | — | Aufbewahrungsfrist |

---

### Prozesse (`prozesse/proc-*.md`)

```markdown
---
id: proc-63-001
titel: Baugenehmigung beantragen
status: aktiv

zustaendigeEinheit: oe-amt-63
zustaendigeRolle: Sachbearbeitung Baurecht

beteiligte:
  - einheit: oe-amt-60
    aufgabe: Naturschutzrechtliche Prüfung

daten:
  input:
    - Bauantrag mit Unterlagen
    - Lageplan, Bauzeichnungen
  output:
    - Baugenehmigung oder Ablehnungsbescheid
  datenspeicher:
    - id: dstore-bauantrag
    - id: dstore-bebauungsplan

regelungen:
  - reg-nbauO-68
  - DSGVO Art. 6 Abs. 1 lit. e

letzte-aktualisierung: 2026-04-01
---

# Baugenehmigung beantragen

## Zweck
...

## Prozessschritte
**01 Antrag prüfen**
*Vollständigkeit und Zulässigkeit des Antrags prüfen.*
...
```

| Feld | Pflicht | Beschreibung |
|---|---|---|
| `id` | ✓ | Stabile ID mit Präfix `proc-` |
| `titel` | ✓ | Anzeigename |
| `status` | ✓ | `aktiv`, `entwurf`, `archiviert` |
| `zustaendigeEinheit` | ✓ | Primär verantwortliche OE |
| `beteiligte` | — | Mitwirkende OEs mit Aufgabe |
| `daten.datenspeicher` | — | Referenzierte Datenarten (IDs aus `daten/`) |
| `regelungen` | — | IDs aus `regelungen/` oder Freitext |

---

### Regelungen (`regelungen/reg-*.md`)

Regelungen folgen dem **ADR-Muster** — nicht nur der Inhalt, sondern auch Kontext und Begründung werden dokumentiert.

```markdown
---
id: reg-adga-001
name: Allgemeine Dienstgebrauchsanweisung
typ: Dienstanweisung
status: aktiv
datum: 2024-01-01

zustaendigeEinheit: oe-stabsstelle
entscheidendes-gremium: Stadtrat

kontext: >
  Gilt für alle Verwaltungsabläufe der Stadtverwaltung.

entscheidung: >
  Eingeführt per Stadtratsbeschluss vom 2024-01-01.

alternativen:
  - Externe Beratung wurde evaluiert, aber abgelehnt
---
```

| Feld | Pflicht | Beschreibung |
|---|---|---|
| `id` | ✓ | Stabile ID mit Präfix `reg-` |
| `name` | ✓ | Anzeigename |
| `typ` | ✓ | Gesetz \| Satzung \| Dienstanweisung \| Richtlinie \| Vertrag \| Beschluss |
| `kontext` | — | Hintergrund und Geltungsbereich (ADR) |
| `entscheidung` | — | Inhalt und Begründung (ADR) |
| `alternativen` | — | Geprüfte und verworfene Alternativen (ADR) |
| `ersetzt` | — | ID der abgelösten Vorgänger-Regelung |

---

## Vokabular — kontrollierte Wertelisten

Der Abschnitt `vokabular` in `koos.yaml` definiert die erlaubten Werte für alle strukturierten Felder. Erweiterungen immer hier eintragen — nie direkt in den Inhaltsdateien erfinden.

### Schutzstufe (Datenschutz — DSGVO / BDSG)

| Stufe | Bedeutung |
|---|---|
| A | öffentlich — keine Schutzmaßnahmen erforderlich |
| B | intern — nur für interne Nutzung; kein personenbezogener Schutzbedarf |
| C | vertraulich — personenbezogene Daten ohne besondere Kategorien |
| D | streng vertraulich — besondere Kategorien nach Art. 9 DSGVO |
| E | geheim — höchster Schutz; Zugang nur namentlich benannten Personen |

### Schutzbedarf (Informationssicherheit — BSI IT-Grundschutz)

| Stufe | Bedeutung |
|---|---|
| normal | Beeinträchtigungen sind begrenzt und überschaubar |
| hoch | Beeinträchtigungen können erheblich sein |
| sehr hoch | Beeinträchtigungen können existenzbedrohend sein |

### Vertraulichkeit (Zugangskontrolle — ISO 27001)

| Stufe | Bedeutung |
|---|---|
| öffentlich | Zur Veröffentlichung freigegeben |
| intern | Nur für Mitarbeitende der Verwaltung |
| vertraulich | Eingeschränkter Personenkreis |
| streng vertraulich | Zugang auf namentlich benannte Personen beschränkt |

Die drei Klassifizierungsachsen sind **unabhängig**:

| Achse | Norm | Frage |
|---|---|---|
| **Schutzstufe** | DSGVO / BDSG | Wie sensibel sind die Daten? |
| **Schutzbedarf** | BSI IT-Grundschutz | Welchen Schaden verursacht ein Sicherheitsvorfall? |
| **Vertraulichkeit** | ISO 27001 | Wer darf die Daten sehen? |

---

## Rollenmodell in orga.yaml

KOOS unterscheidet drei Ebenen von Rollen:

### Ebene 1 — Generische Rollen

Drei Rollen gelten implizit in jeder OE, global in `koos.yaml` hinterlegt:

| Rolle | Bedeutung |
|---|---|
| `Leitung` | Formal verantwortliche Person; Entscheidungs- und Zeichnungsbefugnis |
| `Sachbearbeitung` | Operativ tätig; führt Verwaltungsverfahren durch |
| `Mitarbeitende` | Alle übrigen Personen ohne benannte Funktion |

### Ebene 2 — OE-spezifische Rollen (`rollen:`)

Fachliche Rollen, die nur in einer bestimmten OE vorkommen. Freitext in `orga.yaml`.

### Ebene 3 — Sonderfunktionen (`sonderfunktionen:`)

Gesetzlich definierte Querschnittsfunktionen mit eigener Rechtsgrundlage:

| Funktion | Rechtsgrundlage |
|---|---|
| Datenschutzbeauftragte/r | DSGVO Art. 37, BDSG §38 |
| Informationssicherheitsbeauftragte/r | BSI IT-Grundschutz |
| Gleichstellungsbeauftragte/r | NGG §3 |
| Brandschutzbeauftragte/r | ArbStättV §4 |
| Sicherheitsbeauftragte/r | SGB VII §22 |

**Sonderfall Personalrat:** Der Personalrat ist keine Sonderfunktion, sondern eine eigenständige OE mit eigener ID (`oe-personalrat`). Er ist ein durch NPersVG konstituiertes Gremium ohne Weisungsgebundenheit.

---

## Git als unveränderlicher Speicher

Git übernimmt in KOOS die Rolle des Nix Stores:

- Jeder Commit ist eine **Generation** des Wissensstands.
- Ältere Generationen sind jederzeit wiederherstellbar.
- Freigaben werden als **Tags** markiert (`v2026-Q1`, `nach-reorganisation-2026`).
- Mehrere Verwaltungen können denselben Stand als Ausgangspunkt gabeln.

```bash
git clone https://github.com/dsgvo-dev/koos-daten meine-verwaltung
cd meine-verwaltung
# koos.yaml anpassen → Organisation, Gemeindeschlüssel, Ansprechpartner
# orga.yaml anpassen → eigene Hierarchie
# prozesse/ und daten/ befüllen
```

---

## Regelungen als ADR

Das ADR-Muster (Architecture Decision Records) stammt aus der Softwarearchitektur: Jede wichtige Entscheidung wird als kurzes Dokument festgehalten — mit Kontext, Entscheidung, Begründung und Alternativen.

KOOS überträgt dieses Muster auf Verwaltungsentscheidungen. Eine Regelung dokumentiert nicht nur den INHALT der Entscheidung, sondern deren KONTEXT und BEGRÜNDUNG — das institutionelle Gedächtnis der Verwaltung.

Dieses Prinzip gilt auch innerhalb des KOOS-Servers: Jede Schreiboperation über die Browser-Oberfläche kann mit einer **Begründung** versehen werden, die als Commit-Body im Git-Log festgehalten wird.

---

## Zwei Varianten

KOOS kennt zwei Ausprägungen, die dieselbe Architektur teilen:

| Merkmal | Vereinfacht (dieses Repo) | Vollständig |
|---|---|---|
| Datenpflege | Manuell; Frontmatter + Freitext | Schema-validiert |
| Verknüpfungen | IDs im Klartext | Maschinenlesbare `ref:`-Felder |
| Konsistenzcheck | Keiner — Fehler fallen beim Öffnen auf | Validierung möglich |
| Zielgruppe | Kleine Verwaltungen, Einstieg | Wachsende Systeme, Automatisierung |

Der Übergang von vereinfacht zu vollständig erfordert keine Datenmigration: Die Dateistruktur und das ID-Prinzip sind identisch.

---

## Referenzielle Integrität

In KOOS zeigen alle Verknüpfungen vom Prozess aus nach außen. Die referenzierten Dateien speichern keine Gegenliste. Wird eine Datei gelöscht, entstehen **stille tote Verweise**.

**Option 1 — Soft-Delete (empfohlen):** `status: archiviert` statt physischer Löschung. Verknüpfungen bleiben erhalten und sichtbar.

**Option 2 — Lösch-Guard (geplant):** Der Server prüft vor jeder Löschoperation alle Referenzen:

```
GET /api/referenzen/dstore-personalakte
→ { "prozesse": ["proc-31-001", ...], "count": 336 }
```

**Option 3 — `koos-validate`-Skript:**

```bash
python koos-validate.py
# → WARN: proc-31-001 referenziert dstore-xyz (nicht gefunden)
```

---

## Tradeoffs

| Gewinn | Verlust |
|---|---|
| Keine externe Toolchain — nur Textdateien | Kein automatischer Konsistenzcheck |
| Umbenennung = 1 Zeile; Rückverweise automatisch | IDs müssen beim Anlegen sorgfältig gewählt werden |
| Git-Versionshistorie mit Begründungen | Server muss laufen für Live-Daten |
| BPMN-konformes Datenmodell | Input und Output sind Freitext |
| ADR-Prinzip: Regelungen dokumentieren Kontext | Begründungsfeld ist optional |
| Portabel: Clone = vollständige Instanz | Skalierungsgrenzen bei sehr großen Verwaltungen |
| Lesbar für Menschen und Maschinen | — |

---

## Entwicklungsstand

Abgeschlossen:
- [x] Stabile IDs + Resolver (Inode-Modell)
- [x] Flaches `parent:`-Modell in `orga.yaml`
- [x] Klassifizierung: Schutzstufe, Schutzbedarf, Vertraulichkeit
- [x] Kontrolliertes Vokabular in `koos.yaml`
- [x] Dreistufiges Rollenmodell: generisch / OE-spezifisch / Sonderfunktionen
- [x] BPMN-konformes Datenmodell (Input / Output / Datenspeicher)
- [x] Git-Anbindung — Auto-Init, Commit nach jeder Schreiboperation, Audit-Trail
- [x] **650 Prozesse** als kommunale Verwaltungspraxis-Templates
- [x] **249 Datenarten** im KOOS-Schema

Offen:
- [ ] `regelungen/*.md` — Dienstanweisungen als eigene Dateien (ADR-Muster)
- [ ] Konsistenzcheck-Skript (`koos-validate`)
- [ ] Referenzielle Integrität: Lösch-Guard + Soft-Delete
- [ ] API-Anbindung externer Systeme (OZG-Dienste, Fachverfahren)
- [ ] Übertragung auf weitere Kommunen (Clone-Prozess)

---

## Lizenz

MIT License — siehe [LICENSE](LICENSE)
