---
id: dstore-wohnungsgeberbestaetigung
typ: datenspeicher
system: null
name: Wohnungsgeberbestätigung
datenkategorie: Wohnen & Melderecht
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: BMG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Wohnungsgeber
- Einzug
- Wohnung
- Melderecht
---

# Wohnungsgeberbestätigung

## Definition

Nachweis über den Bezug einer Wohnung zur Anmeldung oder Ummeldung bei der Meldebehörde.

## Felder

- Name Wohnungsgeber
- Anschrift Wohnung
- Einzugsdatum
- Wohnungsart
- Zuordnungsmerkmal
- Bestätigungserteilung

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BMG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Hauptwohnsitz anmelden
- Wohnsitz Anmeldung
- Wohnsitz Abmeldung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
