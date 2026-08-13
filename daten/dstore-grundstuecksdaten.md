---
id: dstore-grundstuecksdaten
typ: datenspeicher
system: null
name: Grundstücksdaten
datenkategorie: Bau & Liegenschaften
zuständige-einheit: oe-amt-63
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: hoch
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: GBO
  - gesetz: NVermG
  aufbewahrung:
    frist: Dauerhaft
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Grundstück
- Kataster
- Grundbuch
- Flurstück
konvertiert-aus: daten1/dtype-grundstuecksdaten.md
---


## Beschreibung

Daten zu Grundstücken aus Kataster und Grundbuch.

## Felder

- Flurstücksnummer
- Gemarkung
- Flur
- Fläche
- Eigentümer
- Grundbuchnummer

## Rechtsgrundlage

GBO, NVermG

## Löschfrist

Dauerhaft

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Grundlage für Beiträge, Genehmigungen und Vermögensverfügungen der Kommune.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei B.** **Sach- und Objektdaten mit mittelbarem Personenbezug.** Gegenstand ist ein Grundstück, ein Bauteil oder ein Behälter; die Person kommt als Eigentümerin, Pflichtige oder Planende hinzu. Aus der Datenart lässt sich nichts über Gesundheit, wirtschaftliche Lage oder Verhalten ableiten. Ein Teil der Angaben ist ohnehin öffentlich zugänglich -- das Baulastenverzeichnis nach § 81 Abs. 3 NBauO wird auf berechtigtes Interesse hin eingesehen, Katasterdaten nach § 12 NVermG.

*Sammelvermerk der Durchsicht vom 2026-08-10.*
