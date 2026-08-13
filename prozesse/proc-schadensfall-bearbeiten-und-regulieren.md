---
id: proc-schadensfall-bearbeiten-und-regulieren
titel: Schadensfall bearbeiten und regulieren (Amtshaftung)
status: aktiv
zustaendigeEinheit: oe-amt-10
zustaendigeRolle: ''
beteiligte:
- einheit: oe-amt-20
  aufgabe: ''
- einheit: oe-amt-66
  aufgabe: ''
daten:
  input: []
  output: []
  datenspeicher:
  - id: dstore-personenstammdaten
  - id: dstore-kontaktdaten
  - id: dstore-bankverbindung
  - id: dstore-kfz-daten
  - id: dstore-gesundheitsdaten
  - id: dstore-sicherheitsmangelmeldung
  - id: dstore-verwaltungsakte
regelungen:
- § 839 Bürgerliches Gesetzbuch (BGB) i. V. m. Art. 34 Grundgesetz (GG) - Amtshaftung
- § 17 Niedersächsisches Straßengesetz (NStrG) - Verkehrssicherungspflicht
- §§ 195, 199 BGB - Verjährung
- Art. 9 Abs. 2 lit. f) DSGVO - Gesundheitsdaten zur Verteidigung von Rechtsansprüchen
- § 3 Niedersächsisches Datenschutzgesetz (NDSG)
leika_id: null
ozg_id: null
letzte-aktualisierung: '2026-07-29'
---

# Schadensfall bearbeiten und regulieren (Amtshaftung)

## Zweck

Bearbeitung von Schadensfällen, in denen **die Kommune als Schädigerin** in Anspruch genommen
wird: Aufnahme der Schadensmeldung, Ermittlung des Sachverhalts, Prüfung der Haftung nach
§ 839 BGB i. V. m. Art. 34 GG, Einschaltung der Haftpflichtversicherung, Entscheidung über
Regulierung oder Ablehnung und Begleitung eines gerichtlichen Verfahrens.

**Abgrenzung nach der Anspruchsrichtung** — das ist bei Schadensfällen der entscheidende
Unterschied:

| Vorgang | Rolle der Kommune | Prozess |
|---|---|---|
| Dritte fordern von der Kommune | **Schädigerin** | dieser Prozess |
| Stadt fordert von Dritten | Geschädigte | `proc-schadensersatz-fuer-die-kommune-geltend-machen` |
| Bürger melden einen Straßenmangel | Trägerin der Verkehrssicherungspflicht | `proc-schaeden-im-strassenbereich-und-an-bruecken-meldung` |

## Prozessschritte

**01 Schadensmeldung aufnehmen**  
*Entgegennahme der Meldung von geschädigten Personen, Zeugen oder dem betroffenen Fachdienst; Aufnahme von Hergang, Ort, Zeit und Schadensumfang*

**02 Sachverhalt ermitteln**  
*Ortsbesichtigung, Fotos und Skizzen, Zeugenbefragung, Stellungnahme des zuständigen Fachdienstes zu Zustand und Kontrollintervallen*

**03 Verkehrssicherungspflicht und Verschulden prüfen**  
*Prüfung, ob eine Amtspflicht verletzt wurde, ob Verschulden vorliegt und ob ein Mitverschulden der geschädigten Person anzurechnen ist*

**04 Haftpflichtversicherung einschalten**  
*Weitergabe des Vorgangs an den Versicherer beziehungsweise den kommunalen Schadensausgleich, Abstimmung der Regulierungsentscheidung*

**05 Über Regulierung entscheiden**  
*Anerkennung oder Ablehnung des Anspruchs, schriftliche Mitteilung mit Begründung an die geschädigte Person*

**06 Zahlung anordnen**  
*Bei Anerkennung Auszahlungsanordnung über die Kasse auf die mitgeteilte Bankverbindung*

**07 Gerichtliches Verfahren begleiten**  
*Bei Klage Zuarbeit für die Prozessvertretung, Zusammenstellung der Unterlagen, Begleitung bis zum rechtskräftigen Abschluss*

**08 Vorgang aufbewahren und löschen**  
*Aufbewahrung nach der Fristenregelung unten; anschließend Vernichtung beziehungsweise Löschung*

## Hinweise

*Angelegt am 2026-07-29 für `vvt-10-010`.*

**Herkunft des Schrittblocks:** abgeleitet aus dem Haftungstatbestand des § 839 BGB i. V. m.
Art. 34 GG und dem Inhalt der `vvt-10-010`, nicht aus einer Ablauferhebung im Amt 10.

**Gesundheitsdaten bei Personenschäden.** Bei einem Personenschaden fallen Angaben zur
ärztlichen Erstversorgung und zum Verletzungsbild an. Das sind Daten nach **Art. 9 DSGVO**.
Die Verarbeitung stützt sich auf **Art. 9 Abs. 2 lit. f) DSGVO** — Geltendmachung, Ausübung
oder Verteidigung von Rechtsansprüchen. Daraus folgen zwei Grenzen: Diese Daten werden nur
erhoben, soweit sie für die Haftungsprüfung erforderlich sind, und sie werden getrennt von den
übrigen Schadensdaten geführt, weil für sie eine eigene Aufbewahrungsfrist gilt.

**Aufbewahrungsfristen (Schritt 08).** Die Fristen richten sich an den Verjährungshöchstfristen
des BGB aus:

| Fall | Frist | Grundlage |
|---|---|---|
| Sachschäden | **10 Jahre** ab Abschluss der Regulierung | § 199 Abs. 3 Nr. 1 BGB |
| Personenschäden | **30 Jahre** | § 199 Abs. 2 BGB |
| anhängiges Verfahren | bis zum rechtskräftigen Abschluss, danach die jeweilige Frist | — |

Die Zehnjahresfrist deckt sich mit `vvt-66-003` und `vvt-34-005`, die beide zehn Jahre führen.

**Keine LeiKa-Nummer:** Die Abwicklung eines Haftungsfalls ist keine Leistung des
Leistungskatalogs.
