---
id: dstore-leitwegid-peppolid
typ: datenspeicher
system: null
name: Leitweg-ID und Peppol-ID
datenkategorie: Finanzen & E-Government
personenbezug: nein   # festgestellt 2026-08-12, siehe Vermerk unten
zuständige-einheit: oe-amt-20
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: ERechV
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-12'
tags:
- Leitweg-ID
- Peppol
---



# Leitweg-ID und Peppol-ID

## Definition

Kennungen für die elektronische Übermittlung strukturierter Rechnungen.

## Felder

- Leitweg-ID
- Peppol-ID
- Gültigkeit
- Zugeordnete Stelle
- Format
- Verwendung

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `hoch`** · **Verfügbarkeit: `normal`**

**Über `normal` gesetzt: Integrität `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Verfügbarkeit bleibt bei `normal`**, geprüft anhand der Fragen des Durchgangs vom 2026-08-04:

1. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

## Personenbezug geprüft 2026-08-12

**Kein Personenbezug.**

Der Speicher führt Leitweg-ID und Peppol-ID. Die **Leitweg-ID** adressiert die Behörde als
Rechnungsempfängerin; die **Peppol-ID** ist eine Netzwerkadresse im Übermittlungsnetz. Das
Feld **„Zugeordnete Stelle"** sagt es selbst: Zugeordnet wird eine Stelle, kein Mensch.

Beide Kennungen werden Rechnungsstellern aktiv bekanntgegeben, damit diese überhaupt
zustellen können.

Nach Art. 4 Nr. 1 DSGVO sind personenbezogene Daten alle Informationen, die sich auf
eine identifizierte oder identifizierbare **natürliche Person** beziehen. Maßgeblich ist
nicht, ob ein Feld einen Namen trägt, sondern **wem der Datensatz zuzuordnen ist**.

Dieser Datensatz ist einer **Organisationseinheit der Kommune** zuzuordnen, nicht einer
natürlichen Person.

Die verwendende Verarbeitung bestätigt das aus zwei Richtungen:

- `vvt-20-004` nennt als Betroffene ausdrücklich *„Lieferanten, Dienstleister und deren
  Vertretungsberechtigte/Ansprechpartner:innen"* — also Personen auf der **Lieferantenseite**.
- Dieselbe Verarbeitung führt unter `kategorien_daten` die Formulierung *„Leitweg-ID und
  Peppol-ID; Rechnungsadressierung **je Organisationseinheit**"*.

## Was daraus folgt

**Die Datenschutz-Schutzstufe ist für diesen Speicher gegenstandslos.** Das
LfD-Schutzstufenkonzept bemisst den Schaden für die betroffene Person; wo es keine gibt, ist
nichts zu bemessen.

**Die BSI-Vektoren bleiben und sind hier der eigentliche Maßstab.** Der Schaden trifft die
Kommune, nicht eine Person: Eine verfälschte Kennung leitet Rechnungen fehl. Die Integrität
steht deshalb seit dem 2026-08-04 auf `hoch`, und das bleibt so.

## Warum die Schutzstufe trotzdem noch dasteht

`klassifizierung.schutzstufe` bleibt vorerst auf **C** — nicht weil sie zutrifft, sondern
weil sie derzeit nicht folgenlos entfernt werden kann:

`besonderheiten_generator.py` liest eine fehlende Schutzstufe als **`A`** und würde diesen
Speicher damit stillschweigend als niedrigste Stufe mitrechnen, statt ihn zu übergehen. Das
ist derselbe Mechanismus, der am 2026-08-10 die gesamte Ableitungskette auf A gezogen hat.
Der Befund dazu:
`documentation/BEFUND-2026-08-12-default-schutzstufe-A-im-generator.md`.

Die Stufe wird entfernt, sobald dieser Default beseitigt ist. Bis dahin ist sie ohne
praktische Wirkung: Alle elf Datenspeicher der `vvt-20-004` stehen auf C, die effektive Stufe
der Verarbeitung bleibt in jedem Fall C.

## Das neue Feld `personenbezug`

`personenbezug: nein` ist am 2026-08-12 neu eingeführt worden und **wird von keinem Skript
ausgewertet**. Es hält die fachliche Feststellung fest, damit sie nicht bei der nächsten
Durchsicht erneut erarbeitet werden muss. Fehlt das Feld, ist damit **keine** Aussage
verbunden — der übrige Bestand ist auf diese Frage nicht durchgesehen.

*Festgestellt bei der Schutzstufendurchsicht Los 3 (Amt 20) am 2026-08-12. Der Speicher bleibt als Datenspeicher bestehen.*
