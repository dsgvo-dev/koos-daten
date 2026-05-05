---
id: dstore-einverstaendnis-sorgeberechtigte
typ: datenspeicher
system: null
name: Einverständnis der Sorgeberechtigten
datenkategorie: Berechtigungsdaten
zuständige-einheit: oe-amt-51
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: BGB
  - gesetz: PAuswG
  - gesetz: PassG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Einverständnis
- Sorgeberechtigte
- Minderjährige
---

# Einverständnis der Sorgeberechtigten

## Definition

Erklärungsdaten, mit denen Sorgeberechtigte einer Antragstellung oder Dokumentenausgabe für Minderjährige zustimmen.

## Felder

- sorgeberechtigte Person
- Art der Zustimmung
- Datum
- Dokumentbezug
- Unterschrift
- Nachweis Sorgeberechtigung

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BGB
- PAuswG
- PassG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Personalausweis – Ausstellung für unter 16-Jährige
- Kinderreisedokumente beantragen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
