---
id: dstore-foerderantrag
typ: datenspeicher
system: null
name: Förderantrag
datenkategorie: Finanzen & Steuern
zuständige-einheit: oe-amt-80
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
  - gesetz: NVwVfG
  - gesetz: Haushaltsrecht
  aufbewahrung:
    frist: 10 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-04'
tags:
- Förderung
- Zuwendung
- Subvention
konvertiert-aus: daten1/dtype-foerderantrag.md
---



## Beschreibung

Antrag auf kommunale Förderung oder Zuwendung.

## Felder

- Antragsteller
- Fördergegenstand
- Fördersumme
- Verwendungsnachweis
- Bewilligungsbescheid

## Rechtsgrundlage

NVwVfG, Haushaltsrecht

## Löschfrist

10 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** An den Vorgang knüpft eine gesetzliche Frist. Ist der Bestand im entscheidenden Zeitraum nicht abrufbar, läuft die Frist gleichwohl -- mit Rechtsfolgen für die Kommune oder die betroffene Person.

Förderfristen sind Ausschlussfristen. Wird ein Verwendungsnachweis nicht rechtzeitig vorgelegt, verfallen bewilligte Mittel -- ein unmittelbarer finanzieller Schaden für die Kommune.
