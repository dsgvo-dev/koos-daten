---
id: dstore-heimbegehung-pruefbericht
typ: datenspeicher
system: null
name: Heimbegehung und Prüfbericht
datenkategorie: Pflegeaufsicht
zuständige-einheit: oe-amt-53
bpmn:
  typ: datenobjekt
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
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c/e
  - gesetz: NuWG
    artikel: §§ 8, 9, 15
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Abschluss der Aufsichtstätigkeit
    hinweis: Festlegung des Trägers
letzte-aktualisierung: '2026-08-15'
tags:
- Heimaufsicht
- Prüfbericht
- Pflegeeinrichtungen
---

# Heimbegehung und Prüfbericht

## Definition

Daten aus Begehungen, Prüfungen und Beschwerden im Rahmen der Aufsicht über
Pflege- und Behinderteneinrichtungen.

## Felder

- Einrichtung
- Begehungstermin
- Feststellungen
- Mängel
- Auflagen
- Halbjahresmeldung

## Schutzstufe geprüft 2026-08-15

**C.** Prüfberichte der Heimaufsicht enthalten Betriebsdaten, Mängel und
Auflagen, aber keine Art. 9-Daten der Bewohner (diese verbleiben im Heim).
Die Daten sind der Einrichtung zugeordnet, nicht einzelnen Bewohnern.
Rechtsgrundlage: NuWG §§ 8, 9, 15.

## BSI-Vektoren geprüft 2026-08-15
