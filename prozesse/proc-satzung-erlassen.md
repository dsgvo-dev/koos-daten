---
id: proc-satzung-erlassen
titel: Satzung erlassen
status: aktiv
zustaendigeEinheit: oe-amt-1-1
zustaendigeRolle: ''
beteiligte:
- einheit: oe-amt-30
  aufgabe: Rechtsförmlichkeitsprüfung des Entwurfs
daten:
  input: []
  output: []
  datenspeicher:
  - id: dstore-verwaltungsakte
regelungen:
- § 10 NKomVG (Satzungsrecht der Gemeinde)
- § 11 NKomVG (Verkündung von Rechtsvorschriften)
letzte-aktualisierung: '2026-08-03'
---

# Satzung erlassen

## Prozessschritte

**01 Erlassbedarf**  
*Politische Entscheidung*

**02 Entwurf erstellen**  
*Rechtssicher formulieren; Rechtsförmlichkeitsprüfung durch Amt 30*

**03 Beschlussfassung**  
*Durch politische Gremien*

**04 Bekanntmachung**  
*In der durch die Hauptsatzung bestimmten Form*

**05 Inkrafttreten**  
*Nach Bekanntmachung*

**06 Verwaltungsvollzug**  
*Umsetzung anweisen*

**07 Überwachung**  
*Einhaltung kontrollieren*

## Abgrenzung zu `proc-bekanntmachungen-veroeffentlichen`

Beide Prozesse gehören zu `vvt-1-1-007`, berühren sich aber nur in Schritt 04. Dieser
Prozess bildet den Rechtsetzungsvorgang von der politischen Entscheidung bis zum
Vollzug ab; `proc-bekanntmachungen-veroeffentlichen` bildet den Verkündungsvorgang als
solchen ab und gilt auch für Bekanntmachungen, die keine Rechtsvorschrift verkünden.

Personenbezug entsteht in diesem Prozess erst mit Schritt 04. Die Schritte 01 bis 03
sind institutionelle Akte; die Schritte 06 und 07 werden in den jeweiligen
Fachverfahren abgebildet, nicht hier.

## Korrekturen 2026-08-03

- **Zuständigkeit von `oe-amt-30` auf `oe-amt-1-1`.** Der Satzungserlass ist keine
  Aufgabe des Rechtsamts. Amt 30 prüft Satzungsentwürfe auf Rechtsförmlichkeit, so wie
  es auch Verträge prüft -- das ist Beteiligung, nicht Zuständigkeit. Amt 30 ist
  entsprechend als beteiligte Einheit mit ausdrücklicher Aufgabe geführt.
- **Verknüpft mit `vvt-1-1-007`** (Öffentliche Bekanntmachungen und Verkündung von
  Ortsrecht). Der Prozess war zuvor mit keiner VVT verknüpft.
- **Regelungsliste bereinigt.** Sie lautete `§§ 10-11 NKomVG (Satzungsrecht der
  Gemeinde)`, `§ 10 BauGB (Bebauungspläne als Satzungen)`, `§ 11 NKomVG
  (Bekanntmachungen)` -- ein Textblock, der wortgleich auch in
  `proc-bebauungsplaene-und-sonstige-satzungen` (Amt 61) und
  `proc-rats-und-buergerinformationssystem-inkl-ortsrecht-satzungen` (Amt 1-1) stand.
  Er beschrieb nicht diesen Prozess, sondern war dreifach verteilt. `§ 11 NKomVG` war
  darin doppelt genannt, einmal in der Spanne und einmal einzeln. `§ 10 BauGB`
  gestrichen: Bauleitplanung ist Amt 61 und in `vvt-61-001` abgebildet.
- **`dstore-bescheid` gestrichen.** Eine Satzung ist eine Rechtsvorschrift, kein
  Verwaltungsakt. Der Datenspeicher bleibt bei `vvt-1-1-007` über
  `proc-bekanntmachungen-veroeffentlichen` erhalten.
