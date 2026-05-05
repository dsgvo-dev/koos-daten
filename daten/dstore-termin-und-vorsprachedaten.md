---
id: dstore-termin-und-vorsprachedaten
typ: datenspeicher
system: null
name: Termin- und Vorsprachedaten
datenkategorie: Verfahrensorganisation
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: prozessabhängig
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Termin
- Vorsprache
- Bürgerbüro
---

# Termin- und Vorsprachedaten

## Definition

Daten zur Terminvereinbarung und persönlichen Vorsprache in Verwaltungsverfahren.

## Felder

- Terminart
- Terminzeitpunkt
- Dienststelle
- Vorsprachepflicht
- Personenanzahl
- Bemerkung

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- prozessabhängig

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Personalausweis – Beantragen
- Eheurkunde beantragen
- Terminvereinbarung bei der Stadt Oldenburg

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
