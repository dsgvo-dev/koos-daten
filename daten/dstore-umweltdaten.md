---
id: dstore-umweltdaten
typ: datenspeicher
system: null
name: Umweltdaten
datenkategorie: Umwelt & Gesundheit
zuständige-einheit: oe-amt-60
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
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: BNatSchG
  - gesetz: BImSchG
  - gesetz: WHG
  aufbewahrung:
    frist: 30 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-04'
tags:
- Umwelt
- Naturschutz
- Immissionsschutz
konvertiert-aus: daten1/dtype-umweltdaten.md
---



## Beschreibung

Daten zu Umweltschutzmaßnahmen: Naturschutz, Immissionsschutz, Gewässerschutz.

## Felder

- Schutzgebiet
- Messwerte
- Grenzwerte
- Maßnahmen
- Genehmigung

## Rechtsgrundlage

BNatSchG, BImSchG, WHG

## Löschfrist

30 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit hoch.** Der Bestand dient der Gefahrenabwehr. Ist er verfälscht oder im entscheidenden Moment nicht abrufbar, kann die Kommune ihre Schutzaufgabe nicht erfüllen -- mit möglichen Folgen für Leib und Leben.

Altlasten- und Messwerte sind Grundlage für Sanierungsanordnungen und Nutzungsbeschränkungen. Ein verfälschter Wert kann eine Gefährdung verdecken.
