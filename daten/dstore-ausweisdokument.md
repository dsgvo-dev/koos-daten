---
id: dstore-ausweisdokument
typ: datenspeicher
system: null
name: Ausweisdokument
datenkategorie: Person & Identität
zuständige-einheit: oe-amt-33
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
  - gesetz: DSGVO
    artikel: Art. 6
  - gesetz: PAuswG
  - gesetz: PassG
  aufbewahrung:
    frist: Kontextabhängig
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Ausweis
- Personalausweis
- Reisepass
- eID
konvertiert-aus: daten1/dtype-ausweisdokument.md
---



## Beschreibung

Amtliches Ausweisdokument: Personalausweis, Reisepass, eID-Karte.

## Felder

- Dokumenttyp
- Dokumentnummer
- Ausstellungsdatum
- Ablaufdatum
- Ausstellende Behörde

## Rechtsgrundlage

Art. 6 DSGVO, PAuswG, PassG

## Löschfrist

Kontextabhängig

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** An den Vorgang knüpft eine gesetzliche Frist. Ist der Bestand im entscheidenden Zeitraum nicht abrufbar, läuft die Frist gleichwohl -- mit Rechtsfolgen für die Kommune oder die betroffene Person.

Ausweis und Pass werden am Schalter ausgegeben; ein Ausfall bedeutet abgewiesene Bürgerinnen und Bürger und verpasste Reisetermine.

## Schutzstufe geprüft 2026-08-10

**D → C.** Dokumenttyp, Nummer, Ausstellungs- und Ablaufdatum, ausstellende Behörde -- Verwaltungsdaten über ein Dokument, keine Aussage über die Person.

**Die Ausweisnummer verdient dennoch Aufmerksamkeit:** § 1 Abs. 2 PAuswG untersagt ihre Verwendung als allgemeines Ordnungsmerkmal und die Bildung von Dateien nach ihr. Das ist eine Anforderung an die Ausgestaltung der Fachverfahren, nicht an die Schutzstufe.

Die sensiblen Bestandteile des Ausweisverfahrens sind eigene Speicher und bleiben auf D: `dstore-biometrische-daten-lichtbild` und `dstore-fingerabdruckdaten` -- biometrische Daten zur eindeutigen Identifizierung nach Art. 9 Abs. 1 DSGVO.
