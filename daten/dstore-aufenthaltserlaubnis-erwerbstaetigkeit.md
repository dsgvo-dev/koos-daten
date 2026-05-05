---
id: dstore-aufenthaltserlaubnis-erwerbstaetigkeit
typ: datenspeicher
system: null
name: Aufenthaltserlaubnis Erwerbstätigkeit
datenkategorie: Migration & Arbeit
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
- Aufenthaltserlaubnis
- Arbeit
- Beschäftigung
---

# Aufenthaltserlaubnis Erwerbstätigkeit

## Definition

Daten zur aufenthaltsrechtlichen Erlaubnis für Beschäftigung oder selbständige Tätigkeit.

## Felder

- Person
- Arbeitgeber oder Tätigkeit
- Erlaubnisumfang
- Befristung
- Nebenbestimmungen
- Nachweise

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
