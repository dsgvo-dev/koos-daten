---
id: dstore-arbeitsunfaehigkeit-krankheit
typ: datenspeicher
system: null
name: Arbeitsunfähigkeit und Krankheit
datenkategorie: Gesundheit & Soziales
zuständige-einheit: oe-amt-53
bpmn:
  typ: nachricht
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: SGB V
  - gesetz: BEEG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Arbeitsunfähigkeit
- Krankheit
- Bescheinigung
---

# Arbeitsunfähigkeit und Krankheit

## Definition

Nachweise über krankheitsbedingte Arbeitsunfähigkeit oder gesundheitliche Einschränkungen, soweit sie verfahrensrelevant sind.

## Felder

- Beginn Arbeitsunfähigkeit
- Ende Arbeitsunfähigkeit
- ärztliche Bescheinigung
- Diagnosehinweis
- Bezug zur Leistung
- Nachweisdatei

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: nachricht

## Rechtsgrundlagen

- SGB V
- BEEG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Elterngeld beantragen
- Hilfe zur Gesundheit

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
