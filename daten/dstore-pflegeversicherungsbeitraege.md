---
id: dstore-pflegeversicherungsbeitraege
typ: datenspeicher
system: null
name: Pflegeversicherungsbeiträge
datenkategorie: Gesundheit & Soziales
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: SGB XI
  - gesetz: SGB XII
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Pflegeversicherung
- Beiträge
- Zuschuss
---

# Pflegeversicherungsbeiträge

## Definition

Beitragsdaten zur Pflegeversicherung für Leistungs- oder Zuschussverfahren.

## Felder

- Pflegeversicherung
- monatlicher Beitrag
- Versicherungsnummer
- Beitragszeitraum
- Leistungsstatus
- Bescheinigung

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- SGB XI
- SGB XII

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Zuschüsse zu Beiträgen für Krankenversicherung und Pflegeversicherung beantragen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
