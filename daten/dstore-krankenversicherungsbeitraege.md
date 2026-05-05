---
id: dstore-krankenversicherungsbeitraege
typ: datenspeicher
system: null
name: Krankenversicherungsbeiträge
datenkategorie: Gesundheit & Soziales
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: SGB V
  - gesetz: SGB XII
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Krankenversicherung
- Beiträge
- Zuschuss
---

# Krankenversicherungsbeiträge

## Definition

Beitragsdaten zur Krankenversicherung für Leistungs- oder Zuschussverfahren.

## Felder

- Krankenversicherung
- Tarif oder Mitgliedschaft
- monatlicher Beitrag
- Versicherungsnummer
- Beitragszeitraum
- Bescheinigung

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- SGB V
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
