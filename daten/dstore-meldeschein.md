---
id: dstore-meldeschein
typ: datenspeicher
system: null
name: Meldeschein
datenkategorie: Wohnen & Melderecht
zuständige-einheit: oe-amt-33
bpmn:
  typ: nachricht
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: BMG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Meldeschein
- Meldeformular
- Anmeldung
---

# Meldeschein

## Definition

Formular- und Erklärungsdaten, die bei An-, Um- oder Abmeldung eines Wohnsitzes erfasst werden.

## Felder

- Meldedatum
- bisherige Anschrift
- neue Anschrift
- Einzugsdatum
- Wohnstatus
- Unterschrift

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: nachricht

## Rechtsgrundlagen

- BMG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Hauptwohnsitz anmelden
- Wohnsitz Abmeldung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
