---
id: dstore-gebuehrenbescheid-zahlungsdaten
typ: datenspeicher
system: null
name: Gebührenbescheid und Zahlungsdaten
datenkategorie: Finanzen & Zahlung
zuständige-einheit: oe-amt-20
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: VwKostR
  - gesetz: Kommunalabgabenrecht
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Gebühr
- Bescheid
- Zahlung
---

# Gebührenbescheid und Zahlungsdaten

## Definition

Bescheid- und Zahlungsdaten zu Gebühren im Verwaltungsverfahren.

## Felder

- Gebührenart
- Betrag
- Bescheiddatum
- Fälligkeit
- Kassenzeichen
- Zahlungsstatus

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- VwKostR
- Kommunalabgabenrecht

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Geburtsurkunde beantragen
- Eheurkunde beantragen
- Baugenehmigung Erteilung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
