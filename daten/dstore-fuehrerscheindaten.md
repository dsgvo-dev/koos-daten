---
id: dstore-fuehrerscheindaten
typ: datenspeicher
system: null
name: Führerscheindaten
datenkategorie: Ordnung & Sicherheit
zuständige-einheit: oe-amt-34
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
  - gesetz: FeV
  - gesetz: StVG
  aufbewahrung:
    frist: 10 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-04'
tags:
- Führerschein
- Fahrerlaubnis
- KFZ
konvertiert-aus: daten1/dtype-fuehrerscheindaten.md
---



## Beschreibung

Daten zur Fahrerlaubnis: Klassen, Ausstellungsdatum, Einschränkungen.

## Felder

- Fahrerlaubnisklassen
- Ausstellungsdatum
- Ablaufdatum
- Einschränkungen
- Führerscheinnummer

## Rechtsgrundlage

FeV, StVG

## Löschfrist

10 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Sie entscheiden über die Berechtigung zum Führen eines Fahrzeugs und stehen im Fahreignungsregister.
