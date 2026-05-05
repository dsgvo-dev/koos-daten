---
id: dstore-geburtsdaten-kind
typ: datenspeicher
system: null
name: Geburtsdaten eines Kindes
datenkategorie: Personenstandsdaten
zuständige-einheit: oe-amt-31
bpmn:
  typ: nachricht
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: PStG
  - gesetz: PStV
  - gesetz: BEEG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Kind
- Geburt
- Geburtsurkunde
- Hausgeburt
- Geburtsanzeige
---

# Geburtsdaten eines Kindes

## Definition

Daten zur Geburt eines Kindes für Registereinträge, Urkunden und familienbezogene Leistungsansprüche.

## Felder

- Vorname des Kindes
- Familienname des Kindes
- Geburtsdatum
- Geburtszeit
- Geburtsort
- Geburtsnachweis

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: nachricht

## Rechtsgrundlagen

- PStG
- PStV
- BEEG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Geburt, Anzeige
- Hausgeburt Anzeige
- Urkunde, Geburtsurkunde/Geburtenregister, Beantragung
- Elterngeld, Antrag

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Kindbezogene Daten wurden von Eltern- und Registerbezug getrennt, um Wiederverwendung zu erleichtern.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
