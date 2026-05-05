---
id: dstore-gesundheitszeugnis-heilpraktiker
typ: datenspeicher
system: null
name: Gesundheitszeugnis Heilpraktiker
datenkategorie: Gesundheit & Erlaubnisse
zuständige-einheit: oe-amt-53
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: HeilprG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Heilpraktiker
- Gesundheitszeugnis
- Erlaubnis
---

# Gesundheitszeugnis Heilpraktiker

## Definition

Gesundheitsbezogene Nachweise im Zulassungsverfahren für Heilpraktikerinnen und Heilpraktiker.

## Felder

- Bescheinigungsart
- ausstellende Stelle
- Ausstellungsdatum
- gesundheitliche Eignung
- Befundhinweis
- Nachweisdatei

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- HeilprG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Sektorale Heilpraktikererlaubnis für Physiotherapie

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
