---
id: dstore-sepa-lastschriftmandat
typ: datenspeicher
system: null
name: SEPA-Lastschriftmandat
datenkategorie: Finanzen & Zahlung
zuständige-einheit: oe-amt-20
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: SEPA-Regelwerk
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- SEPA
- Lastschrift
- Mandat
---

# SEPA-Lastschriftmandat

## Definition

Mandatsdaten zur Einziehung von Gebühren oder laufenden Abgaben per Lastschrift.

## Felder

- Mandatsreferenz
- Gläubiger-ID
- Kontoinhaber
- IBAN
- Erteilungsdatum
- Unterschrift

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- SEPA-Regelwerk

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Hundesteuer – Erhebung
- Bewohnerparkausweis, Erst- und Folgeausstellung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
