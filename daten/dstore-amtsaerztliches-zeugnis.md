---
id: dstore-amtsaerztliches-zeugnis
typ: datenspeicher
system: null
name: Amtsärztliches Zeugnis
datenkategorie: Gesundheit & Erlaubnisse
zuständige-einheit: oe-amt-53
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: prozessabhängig
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- amtsärztlich
- Zeugnis
- Gesundheit
---

# Amtsärztliches Zeugnis

## Definition

Zeugnis oder Stellungnahme einer amtsärztlichen Stelle zur gesundheitlichen Eignung oder zu einem Befund.

## Felder

- ausstellende Stelle
- Ausstellungsdatum
- Zweck
- Eignungsergebnis
- Befristung
- Aktenzeichen

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- prozessabhängig

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Sektorale Heilpraktikererlaubnis für Physiotherapie
- Spielhallenerlaubnis Erteilung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
