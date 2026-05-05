---
id: dstore-wohnungszuordnungsmerkmal
typ: datenspeicher
system: null
name: Wohnungszuordnungsmerkmal
datenkategorie: Wohnen & Melderecht
zuständige-einheit: oe-amt-64
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: BMG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Zuordnungsmerkmal
- Wohnung
- Meldeportal
---

# Wohnungszuordnungsmerkmal

## Definition

Technisches oder organisatorisches Merkmal zur eindeutigen Zuordnung einer Wohnung im Meldeverfahren.

## Felder

- Zuordnungsmerkmal
- Objektkennung
- Wohnungs-ID
- Anschrift
- Vergabestelle

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BMG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Wohnungsgeberbestätigung
- Hauptwohnsitz anmelden

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
