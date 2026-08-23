---
id: dstore-jugendhilfeakte
typ: datenspeicher
system: null
name: Jugendhilfeakte
zuständige-einheit: oe-amt-51
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: E
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: sehr hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: sehr hoch
  rechtsgrundlagen:
  - gesetz: SGB VIII
  aufbewahrung:
    frist: 10–70 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Jugendhilfe
- SGB VIII
- Kind
- Jugend
konvertiert-aus: daten1/dtype-jugendhilfeakte.md
---



## Beschreibung

Dokumentation von Jugendhilfemaßnahmen nach SGB VIII.

## Felder

- Kind/Jugendlicher
- Sorgeberechtigte
- Hilfeplan
- Maßnahmen
- Fachkraft

## Rechtsgrundlage

SGB VIII

## Löschfrist

10–70 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Der Bestand ist Grundlage einer Entscheidung über einen Menschen. Eine unbemerkte Verfälschung führt zu einer falschen Entscheidung, die für die betroffene Person unmittelbare Folgen hat und im Nachhinein kaum aufzuklären ist.

Die Akte trägt Hilfeplanung, Inobhutnahme und Stellungnahmen an das Familiengericht. Eine verfälschte oder lückenhafte Akte führt zu einer falschen Entscheidung über ein Kind. Bei Schutzstufe E ist die Integrität bisher auf „normal" gestanden -- das war die auffälligste Lücke des Katalogs.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei E.** Die Akte nach dem SGB VIII führt Hilfeplan, Maßnahmen und die Angaben zur Familie zusammen. Sie entsteht regelmäßig aus einer Gefährdungsmeldung nach § 8a SGB VIII und dokumentiert, was in einer Familie geschehen ist.

**Stufe E, weil die Offenlegung Menschen gefährden kann:** Wird einem gewalttätigen Elternteil bekannt, was das Kind der Fachkraft berichtet hat oder wo eine Inobhutnahme nach § 42 SGB VIII das Kind untergebracht hat, ist die körperliche Unversehrtheit bedroht. Es gilt der besondere Vertrauensschutz des § 65 SGB VIII, der die Weitergabe anvertrauter Daten selbst innerhalb der Behörde einschränkt.
