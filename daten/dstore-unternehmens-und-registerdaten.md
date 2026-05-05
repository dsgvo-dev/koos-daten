---
id: dstore-unternehmens-und-registerdaten
typ: datenspeicher
system: null
name: Unternehmens- und Registerdaten
datenkategorie: Gewerbe & Organisation
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: HGB
  - gesetz: BGB
  - gesetz: GewO
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Handelsregister
- Vereinsregister
- juristische Person
- Vertreter
- Satzung
---

# Unternehmens- und Registerdaten

## Definition

Daten zu juristischen Personen, Vereinen und deren registerrechtlicher Einordnung.

## Felder

- Rechtsform
- Handelsregisterauszug
- Vereinsregisterauszug
- gesetzlicher Vertreter
- Satzung
- Unternehmensname

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: datenspeicher

## Rechtsgrundlagen

- HGB
- BGB
- GewO

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Spielhallen, Erlaubnis
- Veranstaltung eines Jahr- oder Spezialmarktes: Festsetzung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Organisationsdaten werden separat von Zuverlässigkeitsauskünften geführt, um Unternehmen und Personen trennscharf abzubilden.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
