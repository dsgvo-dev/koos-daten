---
id: dstore-reisekosten-aufenthaltsverfahren
typ: datenspeicher
system: null
name: Reisekosten Aufenthaltsverfahren
datenkategorie: Migration & Kosten
zuständige-einheit: oe-amt-47
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: AufenthG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Reisekosten
- Aufenthalt
- Vorsprache
---

# Reisekosten Aufenthaltsverfahren

## Definition

Kosten- und Erstattungsdaten im Zusammenhang mit ausländerrechtlichen Verfahren.

## Felder

- Reiseanlass
- Strecke
- Betrag
- Nachweis
- Person
- Datum

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
