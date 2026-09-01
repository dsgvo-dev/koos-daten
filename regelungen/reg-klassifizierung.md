---
id: reg-klassifizierung
name: Richtlinie zur Datenklassifizierung
zustaendigeEinheit: oe-amt-1-5
datum: "2026-06-08"
typ: Richtlinie
status: entwurf
freigegeben: 2026-07-10
version: 0.3
freigegeben_v03: 2026-08-12
aenderungen_seit_v02:
  - "Anlage C berichtigt: Schutzstufe C entspricht der BSI-Kategorie *normal*, nicht *hoch*. Grundlage BSI-Standard 200-2 Kap. 8.2.1, Schadensszenario 2 — 'beeinträchtigt' = normal, 'erheblich beeinträchtigt' = hoch, 'Gefahr für Leib und Leben' = sehr hoch"
  - "Anlage C um die Herleitung aus dem BSI-Wortlaut und um die Ausfallzeit-Schwellen der Verfügbarkeit ergänzt"
  - "VIER-ACHSEN-MODELL eingeführt (Kapitel 0, 2.7a, 2.7b, 3, Anlage C): Der BSI-Schutzbedarf ist eine EIGENE Achse, kein Mapping der Achsen 1 und 2 — er misst den Schaden für die verantwortliche Organisation. Fünf der sechs BSI-Schadensszenarien betreffen die Organisation, nur Szenario 2 die betroffene Person"
  - "Vierte Achse aufgenommen: VS-Einstufung nach § 7 VSA Niedersachsen — Schaden für die Interessen des Bundes oder eines Landes, mit der GEGENLÄUFIGEN Zweifelsregel des § 1 Abs. 1 VSA"
  - "Grundsatz ergänzt: Keine Achse wird aus einer anderen abgeleitet"
  - "Ziffer 3.3: Schutzbedarf ist das Maximum ALLER VIER Achsen, nicht zweier"
  - "Klarstellung der Maßstäbe: Datenschutz-Schutzbedarf = Schaden für die betroffene Person; BSI-Schutzbedarf = Schaden für die verantwortliche Organisation"
aenderungen_seit_v01:
  - "LfD-Nds-Schutzstufen korrekt zugeordnet: Art-9-DSGVO-Daten gehören zu D, Stufe E nur Gesundheit/Leben/Freiheit"
  - "Neue Anlage B: Umgangsmatrix (Ablage, Cloud, Mobil, Ausdruck, Übermittlung, Löschung)"
  - "Anlage A (dstore-Tabelle) entsprechend nachgezogen"
  - "Abschnitt 3.4 (Mapping zur DA E-Mail) korrigiert"
  - "Neuer Abschnitt 3.5: Aggregations-/Mischbestandsregel"
  - "Neuer Abschnitt 4.6: Need-to-Know und Data Minimization"
  - "Neuer Abschnitt 6.6: Berufs- und Amtsgeheimnisse (§ 203 StGB, § 30 AO, § 35 SGB I)"
  - "Anlage C (BSI-Mapping) um Erläuterung der bewussten 2-Klassen-Wahl ergänzt"
  - "Anlage E: DIN-66399-Mapping detailliert"
basierend_auf:
  - "Vorgehensweise (dsms:vorgehensweise/Datenschutz-Vorgehensweise.md) — Schutzbedarf normal/hoch"
  - "LfD Niedersachsen — Schutzstufenkonzept A–E (Stand Oktober 2018)"
  - "BSI-Standard 200-2 — IT-Grundschutz-Methodik (Schutzbedarfsfeststellung)"
  - "ISO/IEC 27002:2022, Kapitel 5.12 (Klassifizierung von Informationen)"
  - "DSK-Kurzpapier Nr. 18 — Risiko für die Rechte und Freiheiten"
  - "ISMS-Ratgeber Wiki — Klassifizierung (CC0)"
  - "Konzept VVT/Risiko/DSFA/TOMs (dsms:_archive/bericht-planung-2026-08-15/)"
rechtsgrundlagen:
  - "DSGVO Art. 5 Abs. 1 lit. f (Integrität, Vertraulichkeit)"
  - "DSGVO Art. 9 (besondere Kategorien)"
  - "DSGVO Art. 10 (Strafrechtliche Daten)"
  - "DSGVO Art. 24, 32 (TOMs)"
  - "NDSG (Niedersächsisches Datenschutzgesetz)"
  - "SGB X § 67 (Sozialdaten)"
  - "StGB § 203 (Verletzung von Privatgeheimnissen)"
  - "AO § 30 (Steuergeheimnis)"
  - "SGB I § 35 (Sozialgeheimnis)"
verzahnt_mit:
  - "reg-da-e-mail (DA E-Mail)"
  - "reg-da-cloud (DA Cloud)"
  - "reg-adga (ADGA — Datenschutz/Geheimhaltung)"
  - "reg-isl (Informationssicherheitsleitlinie)"
  - "_daten/daten/dstore-*.md (Datenkategorien)"
  - "dsms:facts/verwaltungsvorschriften/niedersachsen/vsa-verschlusssachenanweisung.md (VSA, dritte Achse)"
  - "dsms:facts/BSI/BSI-Standard-200-2-IT-Grundschutz-Methodik.pdf (Kap. 8.2.1)"
  - "dsms:toms/ (TOM-Bestand)"
---

# Richtlinie zur Datenklassifizierung

## für die [Stadt/Gemeinde/Landkreis] [NAME]

**Erlassen von der Behördenleitung am:** [DATUM]
**Inkrafttreten:** [DATUM]
**Verantwortlich für Fortschreibung:** Stabsstelle Informationssicherheitsbeauftragte/r (ISB)
**Ersetzt:** —

---

## 0. Zweck dieser Richtlinie und Verhältnis zum DSMS

Diese Richtlinie schließt eine Lücke zwischen der **Vorgehensweise** des DSMS (binärer Schutzbedarf „normal" / „hoch") und den **Dienstanweisungen** der Verwaltung (insbesondere DA E-Mail und DA Cloud), die feinere Stufen benötigen, um zwischen „darf per unverschlüsselter Mail raus" und „darf nur über EGVP" zu unterscheiden. Für die Cloud-Nutzung ist die Datenkategorisierung entscheidend, da bestimmte Datenarten nicht oder nur gesichert in Cloud-Umgebungen übertragen werden dürfen.

**Die Dienstanweisung E-Mail-Nutzung** verweist auf diese Richtlinie und die hier definierten Schutzstufen und schreibt für jede Stufe eine zulässige Übertragungsart vor. Analog dockt die DA Cloud, die zukünftige Mobile-Working-Regelung und das Aktenführungs-Regime an die hier definierten Stufen an.

Sie schafft **keine neue Klassifizierungs-Logik**, sondern integriert bereits etablierte. Maßgeblich sind **vier Achsen**, die sich darin unterscheiden, **wem der Schaden droht** — und **ein Ergebnis**, das das Verfahren steuert:

| | Achse | Skala | Geschütztes Gut |
|---|---|---|---|
| 1 | **Schutzstufe** (LfD Niedersachsen, Stand Oktober 2018) | A–E | die **betroffene Person** |
| 2 | **Vertraulichkeitsstufe** (ISO/IEC 27002:2022, Kap. 5.12) | V1–V4 | der **Geheimhaltungsbedarf der Verwaltungsinformation** |
| 3 | **BSI-Schutzbedarf** je Schutzziel (BSI-Standard 200-2, Kap. 8.2.1) | normal · hoch · sehr hoch | die **verantwortliche Organisation** |
| 4 | **VS-Einstufung** (VSA Niedersachsen, § 7) | VS-NfD bis STRENG GEHEIM | die **Interessen des Bundes oder eines Landes** |

**Keine Achse wird aus einer anderen abgeleitet.** Jede ist eigenständig festzulegen.

Der **Schutzbedarf nach Vorgehensweise** (normal/hoch) ist keine Achse, sondern das **Ergebnis**: Er folgt aus dem Maximum aller Achsen und bestimmt das Vorgehen im DSMS — Baseline-TOMs bei „normal", ergänzende Risikoanalyse und ggf. DSFA bei „hoch".

Kapitel 3 setzt die Achsen zueinander in Bezug; **Anlage C** führt Achse 3 und Achse 4 im Einzelnen aus.

---

## 1. Geltungsbereich

1.1 **Persönlicher Geltungsbereich.** Diese Richtlinie gilt für alle Beschäftigten der Verwaltung im Sinne von Abschnitt 2 der ADGA (`reg-adga.md`), einschließlich externer Dienstleister mit Zugriff auf Informationen der Verwaltung.

1.2 **Sachlicher Geltungsbereich.** Sie gilt für alle **Informationen**, die im Rahmen dienstlicher Tätigkeit verarbeitet werden — unabhängig vom Träger (Papier, elektronische Datei, E-Mail, Fachverfahren, Cloud-Dienst, mündliche Mitteilung).

1.3 **Verhältnis zu anderen Regelungen.**
- Vorgehensweise des DSMS — methodische Grundlage (Schutzbedarf).
- Dienstanweisung E-Mail (`reg-da-e-mail.md`) — Anwendung der Schutzstufen auf die Übertragung per E-Mail.
- Dienstanweisung Cloud (`reg-da-cloud.md`) — Anwendung der Schutzstufen auf Cloud-Speicherung und -Verarbeitung.
- ADGA, Abschnitt 9 — allgemeine Grundsätze zu Datenschutz und Informationssicherheit.
- Informationssicherheits-Leitlinie — sicherheitspolitischer Rahmen.

---

## 2. Begriffe

2.1 **Information** — jeder dienstliche Inhalt, unabhängig von Form und Träger.

2.2 **Personenbezogene Daten** — alle Informationen, die sich auf eine identifizierte oder identifizierbare natürliche Person beziehen (Art. 4 Nr. 1 DSGVO).

2.3 **Besondere Kategorien personenbezogener Daten** — Art. 9 Abs. 1 DSGVO (Gesundheit, Sexualleben, ethnische Herkunft, politische Meinungen, religiöse/weltanschauliche Überzeugungen, biometrische Daten zur Identifizierung, genetische Daten, Gewerkschaftszugehörigkeit) sowie Daten zu Straftaten und Verurteilungen (Art. 10 DSGVO).

2.4 **Sozialdaten** — § 67 SGB X.

2.5 **Schutzbedarf** — Maß der Schutzwürdigkeit der Information im Sinne der DSMS-Vorgehensweise. Zwei Klassen: **„normal"** und **„hoch"** (vgl. Anlage C zur Begründung der Zwei-Klassen-Wahl).

2.6 **Schutzstufe** — fünfstufige Klassifizierung personenbezogener Daten nach LfD Niedersachsen (A–E).

2.7 **Vertraulichkeitsstufe** — vierstufige Klassifizierung für Verwaltungsinformationen aus Sicht der Vertraulichkeit (öffentlich, intern, vertraulich, streng vertraulich) nach ISO/IEC 27002:2022.

2.7a **BSI-Schutzbedarf** — dreistufige Klassifizierung (normal, hoch, sehr hoch) **je Schutzziel** — Vertraulichkeit, Integrität, Verfügbarkeit — nach BSI-Standard 200-2, Kapitel 8.2.1. Maßstab ist der Schaden für die **verantwortliche Organisation**, nicht für die betroffene Person. Nicht zu verwechseln mit dem Schutzbedarf nach Ziffer 2.5.

2.7b **VS-Einstufung** — vierstufige Klassifizierung (VS-NUR FÜR DEN DIENSTGEBRAUCH, VS-VERTRAULICH, GEHEIM, STRENG GEHEIM) nach § 7 der Verschlusssachenanweisung für das Land Niedersachsen. Maßstab ist der Schaden für die **Interessen des Bundes oder eines Landes**. Der Regelfall ist keine Einstufung (§ 1 Abs. 1 VSA).

2.8 **Klassifizierende Stelle** — die fachlich verantwortliche Organisationseinheit für die jeweilige Information (KOOS-`oe-*`).

2.9 **Need-to-Know** — Grundsatz, dass eine Information nur Personen zugänglich gemacht wird, die sie für die Erfüllung ihrer dienstlichen Aufgaben kennen müssen.

2.10 **Aggregation** — Zusammenführung von Einzelinformationen zu einem Gesamtbestand, der einen höheren Schutzbedarf erfordern kann als die Einzelteile.

---

## 3. Klassifizierungs-Schema

Die Richtlinie verwendet **vier parallel laufende Achsen** (Übersicht in Kapitel 0). Dieses Kapitel führt Achse 1 und Achse 2 aus; **Achse 3 (BSI-Schutzbedarf) und Achse 4 (VS-Einstufung) stehen in Anlage C.**

Alle Achsen laufen im binären Schutzbedarf der Vorgehensweise zusammen — aber **keine wird aus einer anderen abgeleitet**.

### 3.1 Achse 1 — Schutzstufen nach LfD Niedersachsen (für personenbezogene Daten)

Wortlaut und Beispiele übernehmen die Definitionen des Schutzstufenkonzepts des LfD Niedersachsen (Stand Oktober 2018):

| Stufe | Definition | Beispiele (LfD-Wortlaut) | Schadensschwere (DSK-Kurzpapier 18) | Bezug Schutzbedarf |
|---|---|---|---|---|
| **A** | Personenbezogene Daten, die die Betroffenen **frei zugänglich gemacht** haben. | Telefonverzeichnis, Wahlvorschlagsverzeichnisse, eigene freizugänglich gemachte Webseite, frei zugängliche soziale Medien | vernachlässigbar | normal |
| **B** | Personenbezogene Daten, deren unsachgemäße Handhabung **keine besondere Beeinträchtigung** erwarten lässt, die aber von den Betroffenen **nicht** frei zugänglich gemacht wurden. | Beschränkt zugängliche öffentliche Dateien, Verteiler für Unterlagen, Grundbucheinsicht, nicht frei zugängliche soziale Medien | geringfügig | normal |
| **C** | Personenbezogene Daten, deren unsachgemäße Handhabung den Betroffenen in seiner gesellschaftlichen Stellung oder in seinen wirtschaftlichen Verhältnissen **beeinträchtigen** könnte („Ansehen"). | Einkommen, Grundsteuer, Ordnungswidrigkeiten | überschaubar | normal (Standard); im Einzelfall hoch |
| **D** | Personenbezogene Daten, deren unsachgemäße Handhabung den Betroffenen in seiner gesellschaftlichen Stellung oder in seinen wirtschaftlichen Verhältnissen **erheblich** beeinträchtigen könnte („Existenz"). | Anstaltsunterbringung, Straffälligkeit, dienstliche Beurteilungen, Arbeitszeugnisse, **Gesundheitsdaten**, Schulden, Pfändungen, **Sozialdaten**, **Daten besonderer Kategorien nach Art. 9 DSGVO** | substantiell | hoch |
| **E** | Personenbezogene Daten, deren unsachgemäße Handhabung **Gesundheit, Leben oder Freiheit** der betroffenen Person beeinträchtigen könnte. | Daten über Personen, die mögliche Opfer einer strafbaren Handlung sein können, Zeugenschutzprogramm | groß | hoch |

**Wichtiger Hinweis zur korrekten Einordnung von Art-9-Daten:** Nach LfD Niedersachsen gehören besondere Kategorien personenbezogener Daten nach Art. 9 DSGVO (insbesondere Gesundheitsdaten, Sozialdaten) zur **Stufe D**, **nicht** zu E. Stufe E ist eng auf Konstellationen zugeschnitten, in denen Leben oder Freiheit der betroffenen Person konkret bedroht ist (Opfer von Straftaten, Zeugen, gefährdete Personen). Diese Trennung ist beim Anwenden konsequent einzuhalten.

**Daten zu Straftaten und Verurteilungen (Art. 10 DSGVO):** „Straffälligkeit" ist im LfD-Original Beispiel für **D**; bei besonderem Bedrohungslagen-Bezug (z. B. Sicherungsverwahrte mit konkreter Gefährdungslage) kann Einzelfall-Einstufung in **E** geboten sein.

**Sondergruppen:** Daten von Kindern und besonders schutzbedürftigen Personen werden im Zweifel eine Stufe höher eingestuft als sie sich abstrakt ergeben würden.

### 3.2 Achse 2 — Vertraulichkeitsstufen (für alle Informationen)

| Stufe | Bezeichnung | Beispiele | Bezug Schutzbedarf |
|---|---|---|---|
| **V1** | Öffentlich | Bekanntmachungen, freigegebene Pressemitteilungen, veröffentlichte Satzungen | — |
| **V2** | Intern | Interner Schriftverkehr ohne personenbezogene oder geheimhaltungsbedürftige Inhalte, organisatorische Mitteilungen, Geschäftsverteilungsplan, Telefonlisten | normal |
| **V3** | Vertraulich | Vergabeunterlagen vor Zuschlag, IT-Sicherheitskonzepte, interne Stellungnahmen mit potenziell rufschädigendem Inhalt, Verhandlungsstrategien | normal bis hoch (Einzelfallprüfung) |
| **V4** | Streng vertraulich | Sicherheitsrelevante Pläne (z. B. KRITIS-Notfallpläne), Polizeiliche/Ordnungsbehördliche Lagen, Verschlusssachen nach VSA-Niedersachsen | hoch |

### 3.3 Zusammenführung — Schutzbedarf nach Vorgehensweise

Der **Schutzbedarf einer Information** ergibt sich aus dem **Maximum aller vier Achsen**:

- Schutzbedarf **„hoch"**, sobald eine Achse es erfordert — Schutzstufe **D oder E**, Vertraulichkeitsstufe **V4** (oder V3 nach Einzelfallprüfung), BSI-Schutzbedarf **hoch oder sehr hoch** in einem der drei Schutzziele, oder eine **VS-Einstufung**.
- Sonst Schutzbedarf **„normal"**.

Damit bleibt die Vorgehensweise (Baseline bei „normal", ergänzende Risikoanalyse + ggf. DSFA bei „hoch") in der gewohnten Logik. Die Klassifizierung liefert nur das **Eingangssignal** dazu.

### 3.4 Verhältnis zur DA E-Mail (`reg-da-e-mail.md`)

Die DA E-Mail führt seit dem 24.08.2026 in § 3 unmittelbar das gemeinsame Schema
**V1 / A** bis **V4 / E**; die Umstellung ist vollzogen. § 3 der DA E-Mail füllt die
Zeile „Übermittlung E-Mail" der Umgangsmatrix in **Anlage B** dieser Richtlinie aus.

Die folgende Tabelle dokumentiert die frühere Zuordnung der abgelösten Bezeichnungen
(Niedrig / Normal / Hoch / Sehr hoch). Sie dient dem Verständnis älterer Fassungen und
ist für die Anwendung nicht mehr maßgeblich.

| Abgelöste DA-E-Mail-Bezeichnung | Schutzstufe (Achse 1) | Vertraulichkeitsstufe (Achse 2) | Zulässige Übertragungsart |
|---|---|---|---|
| Niedrig | A | V1 | unverschlüsselt zulässig |
| Normal | B–C | V2 | Transportverschlüsselung (TLS) verpflichtend |
| Hoch | **D** (einschließlich Art-9-Daten, Sozialdaten, Gesundheitsdaten, Steuerdaten) | V3 | Ende-zu-Ende-Verschlüsselung (S/MIME, PGP) oder De-Mail mit QES; gesetzliche Sondervorgaben (§ 30 AO, § 35 SGB I) bleiben unberührt |
| Sehr hoch | **E** (Leben/Freiheit) | V4 | nur über sichere Behördenpostfächer (EGVP, OSCI); keine offene E-Mail, auch nicht verschlüsselt |

### 3.5 Aggregation und Mischbestände

3.5.1 **Mischbestand.** Enthält ein Dokument oder Datenbestand Informationen mehrerer Stufen, gilt grundsätzlich die **höchste enthaltene Stufe** für das gesamte Objekt. Eine getrennte Behandlung (z. B. separate Anlage statt Einbettung) ist zu prüfen, wenn sie die Klassifizierung niedrig halten würde.

3.5.2 **Aggregation.** Werden Einzelinformationen niedrigerer Stufen zu einem Bericht, einer Statistik oder einer Auswertung **zusammengeführt**, kann der Gesamtbestand eine höhere Stufe erfordern als seine Bestandteile. Beispiel: Adressen (B) plus Schuldnerstatus (D) plus räumliche Aggregation ergeben Stufe D, ggf. Hochstufung auf V3.

3.5.3 **Veröffentlichung von Aggregaten.** Vor jeder Veröffentlichung statistischer Auswertungen ist zu prüfen, ob durch die Aggregation Rückschlüsse auf einzelne Personen möglich werden (k-Anonymität, Zellbesetzungs-Mindestgrößen). Bei Zweifeln Rückfrage an DSB.

3.5.4 **Pseudonymisierte und anonymisierte Daten.**
- **Pseudonymisierte** Daten behalten ihre Schutzstufe; die Pseudonymisierung wirkt als TOM, nicht als Klassifizierungs-Senkung.
- **Anonymisierte** Daten (Re-Identifizierung praktisch ausgeschlossen) sind als A bzw. V1 zu führen, sofern keine Vertraulichkeit anderer Art entgegensteht.

---

## 4. Pflicht zur Klassifizierung

4.1 **Grundsatz.** Jede Information ist von der klassifizierenden Stelle bei Erstellung oder Eingang zu klassifizieren. Die Klassifizierung ist Bestandteil der ordnungsgemäßen Aktenführung (vgl. ADGA, Abschnitt 5.9).

4.2 **Anknüpfung an Datenkategorien.** Für strukturierte Verarbeitungen ist die Schutzstufe bereits am **Datenspeicher** (`koos-daten/daten/dstore-*.md`) zu hinterlegen. Damit erbt jeder VVT-Eintrag, der diesen Datenspeicher verwendet, automatisch die Schutzstufe.

4.3 **Defaults bei Unsicherheit.** Im Zweifel ist die **höhere Stufe** zu wählen. Eine Herabstufung bedarf der Begründung und der Bestätigung durch die zuständige Fachbereichsleitung.

4.4 **Mehrkategorien-Dokumente.** Es gilt die Regel aus 3.5.1.

4.5 **Pseudonymisierung / Anonymisierung.** Es gilt die Regel aus 3.5.4.

4.6 **Need-to-Know und Data Minimization als Querschnittsprinzipien.**
- **Need-to-Know:** Zugriff auf Informationen ab Stufe C / V3 wird ausschließlich nach dienstlicher Notwendigkeit gewährt. Eine Hierarchie- oder Anwesenheits-basierte Zugriffsvergabe ist unzulässig.
- **Data Minimization:** Vor jeder Erhebung und vor jeder internen Weitergabe ist zu prüfen, ob für den Zweck weniger oder weniger sensible Daten ausreichen. Auswertungen und Berichte sollen so wenige personenbezogene Daten wie möglich enthalten.

Beide Prinzipien sind in den TOMs des Verfahrens zu verankern (Rolle-Recht-Konzept, Sparsame Default-Konfigurationen).

---

## 5. Kennzeichnung

5.1 **Schriftverkehr.** In Vorlagen und Schriftverkehr ist die Stufe in Kopf- oder Fußzeile zu vermerken, sofern die Stufe **C, D, E oder V3, V4** vorliegt. Beispiele:

- `Schutzstufe C — vertrauliche Behandlung`
- `Schutzstufe D — erhebliche Beeinträchtigung möglich`
- `Schutzstufe E — besonderer Schutz (Leben/Freiheit)`
- `V4 — streng vertraulich`

5.2 **E-Mails.** In der **Betreffzeile** ist bei Stufen ab C / V3 ein Marker zu setzen: `[C]`, `[D]`, `[E]`, `[V3]`, `[V4]`. Damit erkennt das Mail-Gateway die Stufe und kann eine Verschlüsselungspflicht erzwingen (Regelwerk siehe DA E-Mail Abschnitt 3).

5.3 **Aktenführung.** In Aktenplänen und im DMS ist die Stufe als Metadatum pro Vorgang und pro Dokument zu hinterlegen.

5.4 **Fachverfahren.** Soweit das Fachverfahren keine eigene Klassifizierung kennt, ist die maximale Stufe der dort verarbeiteten Daten in der Verfahrensbeschreibung zu dokumentieren.

5.5 **Stufe A / V1.** Eine Kennzeichnung ist nicht erforderlich; das Fehlen einer Kennzeichnung gilt nicht als A/V1, sondern fordert eine Plausibilitätsprüfung.

---

## 6. Folgen der Klassifizierung

6.1 **Speicherung.** Stufen D, E, V3, V4 sind außerhalb des kommunalen Netzes nur in vom ISB freigegebenen, ggf. verschlüsselten Speicherorten zulässig. Cloud-Nutzung richtet sich nach der DA Cloud. Details siehe **Anlage B (Umgangsmatrix)**.

6.2 **Übermittlung.** E-Mail, Fax, Post, Schnittstellen — Übertragungsweg ist nach Stufe zu wählen. Die DA E-Mail enthält die Detailregelung; **Anlage B** fasst die Anforderungen zusammen.

6.3 **Zugriff.** Stufen D, E, V3, V4 dürfen nur Personen mit dienstlichem Bedarf einsehen (Need-to-Know, vgl. 4.6). Rollen-Rechte-Konzept gemäß TOMs.

6.4 **Aufbewahrung und Löschung.** Die Aufbewahrungsfristen ergeben sich aus dem jeweiligen Fachrecht (vgl. Frontmatter-Feld `loeschfrist` im VVT-Eintrag). Die Klassifizierung bestimmt **nicht** die Frist, wohl aber die Anforderungen an die Vernichtung (vgl. **Anlage E — DIN-66399-Mapping**).

6.5 **Vorfallsmeldung.** Verlust oder Offenlegung von Informationen ab Stufe C / V3 ist als möglicher Datenschutz- bzw. Sicherheitsvorfall der DSB / dem ISB zu melden (ADGA 9.4).

6.6 **Berufs- und Amtsgeheimnisse.** Unabhängig von der Schutzstufe gelten gesetzliche Schweige- und Geheimhaltungspflichten fort, insbesondere:
- **§ 203 StGB** (Verletzung von Privatgeheimnissen) für Beschäftigte in Sozialleistungsbereichen, Jugendamt, Gesundheitsamt, Schwangerenberatung, Schuldnerberatung, Drogenberatung.
- **§ 30 AO** (Steuergeheimnis) im Bereich der kommunalen Steuerverwaltung.
- **§ 35 SGB I** (Sozialgeheimnis) für alle Sozialleistungsträger.
- **VS-Anweisung Niedersachsen** für eingestufte Verschlusssachen.

Die Schutzstufe ersetzt diese Geheimhaltungspflichten nicht; sie verlangen häufig **strengere** Behandlung als die jeweilige Stufe vorgibt. Im Zweifel gilt die strengere Vorgabe.

---

## 7. Verantwortlichkeiten

| Rolle | Aufgabe |
|---|---|
| **Klassifizierende Stelle** (Fachbereich / Sachbearbeitung; Information Owner) | Klassifizierung im Einzelfall, Kennzeichnung, Anwendung der Vorgaben |
| **Fachbereichsleitung** | Plausibilitätsprüfung, Bestätigung von Herabstufungen, Schulung des eigenen Bereichs, Ressourcen für Klassifizierungs-Aufwand bereitstellen |
| **Datenschutzbeauftragte/r (DSB)** | Beratung bei personenbezogenen Daten ab Stufe C, Vorfallsbearbeitung, Fortschreibung der Schutzstufen am `dstore-*`-Bestand |
| **Informationssicherheitsbeauftragte/r (ISB)** | Fortschreibung der Vertraulichkeitsstufen, Abstimmung mit DSB, Vorgaben zu Speicherung und Übertragung, jährliches Klassifizierungs-Audit |
| **IT** | Technische Umsetzung (Mail-Gateway-Regeln, Verschlüsselungs-Infrastruktur, DMS-Metadaten, Zugriffskonzepte) |
| **Verwaltungsleitung** | Erlass und Fortschreibung dieser Richtlinie |

---

## 8. Schulung

8.1 **Erstunterweisung** für alle neu Eintretenden vor Tätigkeitsaufnahme.

8.2 **Jährliche Auffrischung** für alle Beschäftigten; Themenwechsel jährlich (Schutzstufen, E-Mail-Verschlüsselung, Cloud, Mobile Working).

8.3 **Schulungsnachweise** sind in der Personalakte zu führen.

8.4 **Sensibilisierung anhand von Fallbeispielen.** Schulungen enthalten konkrete Fallbeispiele aus der Verwaltungspraxis (Wohnungsgeber, Jugendamt, Steueramt, Bauamt), die die Stufen-Zuordnung üben.

---

## 9. Inkrafttreten und Überprüfung

9.1 **Inkrafttreten.** Diese Richtlinie tritt am [DATUM] in Kraft.

9.2 **Überprüfung.** Sie wird **jährlich** durch DSB und ISB gemeinsam überprüft. Anlassbezogene Anpassung erfolgt insbesondere bei Änderungen der DSGVO, des NDSG, des LfD-Schutzstufenkonzepts oder bei wesentlicher Änderung der Verwaltungs-Infrastruktur.

9.3 **Versionierung.** Diese Richtlinie wird im DSMS (`dsms-knowledge/Muster-Dienstanweisungen/`) versioniert geführt. Versionsstände werden über Git-Tags festgehalten (vgl. KONZEPT VVT/Risiko/DSFA/TOMs, Kapitel 10).

---

## Anlage A — Fallbeispiele zur Schutzstufen-Einordnung (Schulungsmaterial)

Diese Anlage enthält **Übungsbeispiele** zur Anwendung der Entscheidungshilfe aus Anlage D, passend zu Punkt 8.4 (Sensibilisierung anhand von Fallbeispielen). Sie ist **kein Nachschlagewerk** für die tatsächliche Einstufung konkreter IT-Verfahren oder Datenbestände einer Verwaltung — diese Einstufung erfolgt für strukturierte Verarbeitungen ausschließlich am jeweiligen Datenspeicher im Fachverfahren bzw. im KOOS-System (vgl. Punkt 4.2) und ist dort für Berechtigte einsehbar, nicht in dieser Richtlinie.

| Beispiel | Schutzstufe (Achse 1) | Vertraulichkeit (Achse 2) | Schutzbedarf |
|---|---|---|---|
| Stammdaten natürlicher Personen (Name, Anschrift) | B–C | V2 | normal |
| Bestätigung einer Anmeldung/eines Vorgangs | B | V2 | normal |
| Sozialdaten i. S. d. § 67 SGB X | **D** | V3 | hoch |
| Steuerliche Festsetzungsdaten | **D** | V3 | hoch (§ 30 AO) |
| Versicherungsnachweis (z. B. Haftpflicht) | B | V2 | normal |
| Auszug aus dem Bundeszentralregister (Führungszeugnis) | **D** (Art. 10 DSGVO) | V3 | hoch |
| Übermittlungssperre im Melderegister — schützt vor Auskünften | **D** (im Einzelfall **E**, wenn Schutz vor Bedrohung Grund der Sperre) | V3–V4 | hoch |
| Anspruch auf Leistungen für Bildung und Teilhabe | **D** (Sozialleistungsbezug) | V3 | hoch |
| Schilderung eines Schadensereignisses ohne Personenbezug hoher Sensibilität | C | V2 | normal |
| Zahlungsverkehrsdaten (allgemein) | C–**D** (bei Pfändungen, Vollstreckung) | V3 | normal bis hoch |
| Gebührenbescheide | C | V2 | normal |
| Leistungsdaten zur Mutterschaft | **D** (Gesundheits-Bezug, Sozialleistung) | V3 | hoch |
| Staatsangehörigkeit (Art. 9 möglich: ethnische Herkunft) | C–**D** | V2–V3 | normal bis hoch |
| Geburtsdaten von Kindern | C, Hochstufung wegen Schutzbedürftigkeit auf **D** | V2 | hoch |
| Auskunftssperre im Melderegister bei Gefahrenlage (§ 51 BMG) | **E** (in der Regel — Gefahr für Leben/Freiheit) | V4 | hoch |

**Hinweis:** Diese Beispiele sind zur Einübung der Anlage-D-Systematik gedacht, nicht als abschließende oder verbindliche Klassifizierung zu verstehen. Die verbindliche Einstufung eines konkreten Datenbestands nimmt die klassifizierende Stelle nach Anlage D vor bzw. übernimmt sie aus dem Fachverfahren/System, in dem sie hinterlegt ist.

---

## Anlage B — Umgangsmatrix (operationale Vorgaben)

Quelle der Struktur: ISMS-Ratgeber Wiki, „Klassifizierung" (CC0), angepasst auf kommunale Verwaltung. Die Matrix verbindet die Klassifizierung mit den Folgepflichten und ist Anker für DA E-Mail und DA Cloud.

| Aspekt | V1 / A — Öffentlich | V2 / B — Intern | V3 / C–D — Vertraulich | V4 / E — Streng vertraulich |
|---|---|---|---|---|
| **Kreis der Berechtigten** | jede/r | Beschäftigte; bei Bedarf benannte Externe | Beschäftigte mit dienstlichem Bedarf (Need-to-Know) | Einzeln benannte Personen; explizite Freigabe der Leitung |
| **Ablage Papier** | beliebig | im Dienstzimmer | im verschlossenen Schrank, Zutritt geregelt | in zugriffsgeschütztem Bereich (z. B. Tresor, Geheimschutz-Schrank) |
| **Ablage elektronisch — Verwaltungsnetz** | beliebig | reguläre Fachverfahren / Laufwerke | zugriffsgeschützte Verzeichnisse, Rollen-Rechte-Konzept | zusätzlich verschlüsselt, Protokollierung des Zugriffs |
| **Cloud-Speicher** | beliebig zulässig | nur in vom ISB freigegebenen EU-Diensten | nur freigegebene EU-Dienste + zusätzliche Verschlüsselung unter Kontrolle der Verwaltung | **nicht zulässig** außer mit Einzelgenehmigung der Verwaltungsleitung nach ISB-Stellungnahme |
| **Mobile Speicher (USB, Notebook, Smartphone)** | beliebig | nur verschlüsselte, freigegebene Geräte | nur freigegebene und vollverschlüsselte Geräte, sicherer Datentransport | nicht außerhalb des Dienstgebäudes ohne ausdrückliche Freigabe |
| **Ausdruck / Kopie** | beliebig | innerhalb der Verwaltung | nur im notwendigen Umfang im zuständigen Bereich, Vernichtung nach Bedarf | nur mit Zustimmung der Leitung, Kopien zählen |
| **Übermittlung intern (Hauspost)** | offen | offen | verschlossener Umschlag mit Vermerk „vertraulich" | versiegelter Umschlag, persönliche Übergabe |
| **Übermittlung extern Papier** | offen | offen | Einschreiben oder versiegelt | persönliche Übergabe gegen Quittung, ggf. Wertbrief |
| **Übermittlung E-Mail** | unverschlüsselt zulässig | TLS-Transportverschlüsselung (Standard) | Ende-zu-Ende (S/MIME, PGP) oder De-Mail mit QES | nur sichere Behördenpostfächer (EGVP, OSCI); keine E-Mail |
| **Übermittlung Fax** | zulässig | zulässig | nur, wenn Empfänger gesichert (Fax-zu-Mail mit verschlüsselter Zustellung) | unzulässig |
| **Telefonat** | beliebig | beliebig | nur mit Verifikation des Anrufers; sensible Inhalte vermeiden | nur über gesicherte Verbindungen, vorzugsweise persönlich |
| **Bildschirmsperre** | empfohlen | verpflichtend bei Verlassen | verpflichtend, automatisch ≤ 5 Min. | verpflichtend, automatisch ≤ 2 Min., Sichtschutz-Folie empfohlen |
| **Löschung / Vernichtung** | keine Vorgaben | DIN 66399 Stufe 2 (P-3) | DIN 66399 Stufe 4 (P-4 oder höher) | DIN 66399 Stufe 5–6 (P-5/P-6 oder höher); Crypto-Shredding bei elektronischen Trägern |
| **Backup** | regulär | regulär | regulär, verschlüsselt | regulär, verschlüsselt, getrennte Aufbewahrung |
| **Aufbewahrung außerhalb des Hauses** | unkritisch | nur mit ausdrücklicher Freigabe (z. B. Homeoffice) | nur mit Freigabe + verschlüsseltem Speicher | grundsätzlich unzulässig |

**Anwendungsregel:** Die Matrix gilt als Mindeststandard. Fachspezifische strengere Vorgaben (§ 203 StGB, § 30 AO, § 35 SGB I, VSA) gehen vor.

---

## Anlage C — Verhältnis zu BSI-Grundschutz-Schutzbedarf

Der **BSI-Standard 200-2** (IT-Grundschutz-Methodik) kennt drei Schutzbedarfskategorien — **normal, hoch, sehr hoch** — und drei Schutzziele — **Vertraulichkeit, Integrität, Verfügbarkeit**.

Das DSMS dieser Verwaltung arbeitet im Sinne der Vorgehensweise mit **zwei** Klassen — **normal, hoch**. Diese Reduktion ist **bewusst** und wird in der Vorgehensweise (Abschnitt zu „Grundüberlegung 2: Vereinfachung durch Schutzbedarfe ‚normal' und ‚hoch'") begründet:

- Operative Folge der Einstufung ist binär — Baseline-TOMs bei „normal", ergänzende Risikoanalyse plus ggf. DSFA bei „hoch".
- Eine dritte Klasse „sehr hoch" würde keinen zusätzlichen Verfahrensschritt einführen, sondern nur die Risikoanalyse intensivieren — das ergibt sich bereits aus der konkreten Risikobewertung innerhalb von „hoch".
- DSFA und Konsultation der Aufsichtsbehörde nach Art. 36 DSGVO greifen unabhängig von der Anzahl der Klassen, wenn die Schwellwerte des Art. 35 erfüllt sind.

Für die **TOMs aus dem KOOS-TOM-Bestand** bleibt der dreiwertige BSI-Schutzbedarf in der **Beschreibung** der Maßnahme weiterhin nutzbar (Maßnahme X greift bei „sehr hoch" stärker als bei „hoch"). Auf der Ebene der **Verfahrensführung** wird er auf zwei Klassen verdichtet.

### Der BSI-Schutzbedarf ist eine eigene Achse

> **Korrektur v0.3 (2026-08-12) — zwei Punkte.**
>
> **Erstens:** Die vorige Fassung ordnete die Schutzstufe **C** der BSI-Kategorie *hoch* zu. Das widerspricht dem BSI-Original — siehe unten. Der Bestand in `koos-daten/daten/dstore-*.md` war insoweit richtig eingestuft und die Anlage falsch.
>
> **Zweitens, und wichtiger:** Die vorige Fassung behandelte den BSI-Schutzbedarf als **Mapping** zu den Achsen 1 und 2. Das ist falsch. Er misst ein **eigenes Schutzgut** und ist damit eine **eigene Achse**.

Die Klassifizierung kennt **vier Achsen**. Sie unterscheiden sich nicht in der Skala, sondern darin, **wem der Schaden droht**:

| | Instrument | Skala | Geschütztes Gut | Quelle |
|---|---|---|---|---|
| **1** | Schutzstufe | A–E | die **betroffene Person** | LfD Niedersachsen |
| **2** | Vertraulichkeitsstufe | V1–V4 | der **Geheimhaltungsbedarf der Verwaltungsinformation** — wer darf sie kennen | ISO/IEC 27002:2022, Kap. 5.12 |
| **3** | BSI-Schutzbedarf, je Schutzziel | normal · hoch · sehr hoch | die **verantwortliche Organisation** — Aufgabenerfüllung, Ansehen, Finanzen, Rechtstreue | BSI-Standard 200-2, Kap. 8.2.1 |
| **4** | VS-Einstufung | VS-NfD · VS-VERTRAULICH · GEHEIM · STRENG GEHEIM | die **Interessen des Bundes oder eines Landes** | VSA Niedersachsen, § 7 |

**Keine Achse wird aus einer anderen abgeleitet.** Jede ist eigenständig festzulegen. Wer eine aus einer anderen errechnet, lässt sie verschwinden.

### Achse 3 im Einzelnen — BSI-Standard 200-2, Kapitel 8.2.1

Das BSI bestimmt den Schutzbedarf **je Schutzziel** (Vertraulichkeit, Integrität, Verfügbarkeit) anhand von **sechs Schadensszenarien**:

1. Verstoß gegen Gesetze, Vorschriften, Verträge
2. Beeinträchtigung des informationellen Selbstbestimmungsrechts
3. Beeinträchtigung der persönlichen Unversehrtheit
4. Beeinträchtigung der Aufgabenerfüllung
5. Negative Innen- oder Außenwirkung
6. Finanzielle Auswirkungen

**Fünf dieser sechs Szenarien betreffen die Organisation, nicht die betroffene Person.** Nur Szenario 2 hat den Betroffenen im Blick — und dessen Wortlaut ist zufällig deckungsgleich mit den Kriterien des LfD-Konzepts:

| BSI-Kategorie | Wortlaut Szenario 2 | entspricht Schutzstufe |
|---|---|---|
| **normal** | „…der Betroffene in seiner gesellschaftlichen Stellung oder in seinen wirtschaftlichen Verhältnissen **beeinträchtigt** werden kann" | C (und darunter A, B) |
| **hoch** | „…**erheblich beeinträchtigt** werden kann" | D |
| **sehr hoch** | „…eine **Gefahr für Leib und Leben oder die persönliche Freiheit** des Betroffenen gegeben ist" | E |

**Diese Tabelle ist eine Beobachtung, keine Regel.** Sie zeigt, wo sich zwei Achsen in *einem* von sechs Szenarien decken. Der BSI-Schutzbedarf einer Datenart kann aus jedem der anderen fünf Szenarien höher ausfallen — eine Löschwasserkarte ohne jeden Personenbezug hat hohe Verfügbarkeit, ein Melderegister hohe Integrität.

Das BSI selbst zieht die Konsequenz: Szenario 2 **kann entfallen**, „wenn in der Institution das Datenschutzmanagement dieses Szenario bereits ausreichend betrachtet hat". Für abweichende Ergebnisse verweist es auf das SDM.

**Verfügbarkeit ist quantifiziert** (Szenario 4, maximal tolerierbare Ausfallzeit):

| Kategorie | Ausfallzeit |
|---|---|
| normal | 24 bis 72 Stunden |
| hoch | 1 bis 24 Stunden |
| sehr hoch | unter einer Stunde |

### Achse 4 im Einzelnen — Verschlusssachen

Die **VS-Einstufung** nach § 7 VSA Niedersachsen bemisst den Schaden für die Interessen des Bundes oder eines Landes. Sie folgt einer **gegenläufigen Zweifelsregel**: § 1 Abs. 1 VSA — *„Von einer Einstufung als VS ist nur der notwendige Gebrauch zu machen."* Die Achsen 1 bis 3 stufen im Zweifel höher ein (Ziffer 4.3), Achse 4 im Zweifel gar nicht. Der Normalfall kommunaler Datenarten ist **keine** VS-Einstufung.

Anlage 1 Nr. 1 VSA grenzt selbst ab: Für personenbezogene Daten sind *„die hierfür bestehenden Regelungen … anzuwenden"*, nicht die VSA. **Eine hohe Schutzstufe begründet keine VS-Einstufung.**

Ab **VS-VERTRAULICH** werden Sicherheitsüberprüfung aller befassten Personen, materielle Schutzmaßnahmen und eigene IT-Anforderungen ausgelöst; ab dieser Stufe ist eine oder ein Geheimschutzbeauftragte/r zu bestellen (§ 3 VSA).

Erfasst in `dsms-knowledge/facts/verwaltungsvorschriften/niedersachsen/vsa-verschlusssachenanweisung.md`.

### Der Schutzbedarf der Vorgehensweise bleibt binär

Der **DSMS-Schutzbedarf** (normal/hoch) ist keine fünfte Achse, sondern das **Ergebnis**: Er ergibt sich aus dem Maximum aller Achsen und steuert das Verfahren — Baseline-TOMs bei „normal", ergänzende Risikoanalyse und ggf. DSFA bei „hoch". Die Zwei-Klassen-Wahl ist oben begründet.

---

## Anlage D — Entscheidungs-Hilfe für die Sachbearbeitung

Drei Fragen in dieser Reihenfolge:

1. **Sind personenbezogene Daten enthalten?**
   - Nein → nur Achse 2 (V1–V4) anwenden.
   - Ja → weiter zu Frage 2.

2. **Wären die Daten geeignet, Gesundheit, Leben oder Freiheit der betroffenen Person zu gefährden** (z. B. Daten zu Bedrohten, Zeugen, Opfern, Personen mit Auskunftssperre nach Gefährdungslage)?
   - Ja → Stufe **E**. Stopp.
   - Nein → weiter zu Frage 3.

3. **Wären die Daten geeignet, bei Missbrauch die wirtschaftliche Existenz oder gesellschaftliche Stellung der betroffenen Person erheblich zu beeinträchtigen** (z. B. Sozialdaten, Gesundheitsdaten, Art-9-DSGVO-Daten, Strafdaten, Schulden, Pfändungen, dienstliche Beurteilungen)?
   - Ja → Stufe **D**.
   - Beeinträchtigung möglich, aber nicht existenziell (Einkommen, Grundsteuer, Ordnungswidrigkeiten) → Stufe **C**.
   - Nicht frei zugänglich, aber ohne erkennbare Beeinträchtigung → Stufe **B**.
   - Vom Betroffenen frei zugänglich gemacht → Stufe **A**.

Bei Konflikt: höhere Stufe gewinnt, Rückfrage an DSB.

---

## Anlage E — DIN-66399-Mapping (Vernichtung)

Die DIN 66399 unterscheidet sechs Schutzklassen und sieben Sicherheitsstufen (P-1 bis P-7 für Papier; analog für andere Medien). Verwaltungs-typische Zuordnung:

| Schutzstufe (Achse 1) | Vertraulichkeit (Achse 2) | DIN 66399 — Schutzklasse | Sicherheitsstufe Papier | Bemerkung |
|---|---|---|---|---|
| A | V1 | 1 | P-2 | keine besondere Vorgabe |
| B | V2 | 1–2 | P-3 | reguläre Aktenvernichtung |
| C | V2–V3 | 2 | P-4 | Schnitzelgröße ≤ 160 mm² |
| D | V3 | 3 | P-5 | Schnitzelgröße ≤ 30 mm² — vorgeschrieben bei Sozial-, Steuer-, Gesundheits- und Art-9-Daten |
| E | V4 | 3 | P-6 oder P-7 | maximaler Schutz; bei elektronischen Trägern Crypto-Shredding |

Bei elektronischen Trägern gelten die korrespondierenden Stufen der DIN 66399-2 (z. B. E-3 / E-4 für Festplatten).

---

## Anlage F — Glossar (Kurzform)

| Begriff | Bedeutung |
|---|---|
| **Schutzbedarf** | Methodische Größe der Vorgehensweise — „normal" oder „hoch". Steuert, ob Baseline-TOMs ausreichen oder eine ergänzende Risikoanalyse folgt. |
| **Schutzstufe (A–E)** | Klassifizierung **personenbezogener Daten** nach LfD Niedersachsen (Stand Oktober 2018). |
| **Vertraulichkeitsstufe (V1–V4)** | Klassifizierung **aller dienstlichen Informationen** nach Geheimhaltungsbedarf, ISO/IEC 27002:2022. |
| **VS-NfD / VS-VERTRAULICH** | Verschlusssachen nach VS-Anweisung Niedersachsen. Stufe V4 entspricht mindestens VS-NfD. |
| **DSB** | Datenschutzbeauftragte/r |
| **ISB** | Informationssicherheitsbeauftragte/r |
| **DMS** | Dokumentenmanagementsystem |
| **EGVP** | Elektronisches Gerichts- und Verwaltungspostfach |
| **OSCI** | Online Services Computer Interface (Standard für sichere Behördenkommunikation) |
| **DIN 66399** | Norm für die sichere Vernichtung von Datenträgern (Schutzklassen 1–3, Sicherheitsstufen P-1 bis P-7) |
| **Need-to-Know** | Zugriffsprinzip: nur wer die Information dienstlich braucht, erhält Zugriff |
| **Aggregation** | Zusammenführung von Einzelinformationen; kann den Schutzbedarf erhöhen |
| **Crypto-Shredding** | Vernichtung verschlüsselter Daten durch sicheres Löschen des Schlüssels |

---

## Quellen

- DSGVO Artt. 4, 5, 9, 10, 24, 32
- NDSG (Niedersächsisches Datenschutzgesetz)
- StGB § 203, AO § 30, SGB I § 35, SGB X § 67
- LfD Niedersachsen — Schutzstufenkonzept (Stand Oktober 2018) — `lfd.niedersachsen.de/download/137188/Schutzstufenkonzept_LfD_Niedersachsen_.pdf`
- DSK-Kurzpapier Nr. 18 — Risiko für die Rechte und Freiheiten natürlicher Personen
- BSI IT-Grundschutz-Kompendium und BSI-Standard 200-2 (Schutzbedarfsfeststellung)
- ISO/IEC 27002:2022, Kapitel 5.12 (Klassifizierung von Informationen)
- ISMS-Ratgeber Wiki — Klassifizierung (CC0), `wiki.isms-ratgeber.info/wiki/Klassifizierung`
- DIN 66399 — Büro- und Datentechnik, Vernichtung von Datenträgern
- Vorgehensweise — `dsms-knowledge/vorgehensweise/Datenschutz-Vorgehensweise.md`
- Konzept VVT/Risiko/DSFA/TOMs — `dsms-knowledge/Bericht Planung/`
- Dienstanweisung E-Mail, Cloud, ADGA — `dsms-knowledge/Muster-Dienstanweisungen/`
