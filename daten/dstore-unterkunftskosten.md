---
id: dstore-unterkunftskosten
typ: datenspeicher
system: null
name: Unterkunftskosten
datenkategorie: Wohnen & Soziales
zuständige-einheit: oe-amt-64
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: WoGG
  - gesetz: SGB XII
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Unterkunft
- Kosten
- Wohnen
---

# Unterkunftskosten

## Definition

Kostenbezogene Daten zur Unterkunft im Rahmen von Förder- oder Sozialleistungen.

## Felder

- Grundmiete
- Betriebskosten
- Heizkosten
- Warmmiete
- Kostenanteil
- Nachweisart

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- WoGG
- SGB XII

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Wohngeld erstmalig oder neu beantragen
- Zuschüsse zu Beiträgen für Krankenversicherung und Pflegeversicherung beantragen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
