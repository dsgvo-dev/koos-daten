---
id: dstore-kinderbetreuung-kosten
typ: datenspeicher
system: null
name: Kinderbetreuungskosten
datenkategorie: Bildung & Betreuung
zuständige-einheit: oe-amt-51
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: BEEG
  - gesetz: SGB VIII
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Kinderbetreuung
- Kita
- Kosten
---

# Kinderbetreuungskosten

## Definition

Kosten- und Nachweisdaten für Betreuung von Kindern in Einrichtungen oder Tagespflege.

## Felder

- Einrichtung
- Betreuungsumfang
- monatliche Kosten
- Beginn Betreuung
- Kind
- Kostenbescheid

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BEEG
- SGB VIII

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Elterngeld beantragen
- Bildung und Teilhabe beantragen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
