---
id: dstore-wohnraumnachweis-aufenthalt
typ: datenspeicher
system: null
name: Wohnraumnachweis Aufenthalt
datenkategorie: Migration & Aufenthalt
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
- Wohnraum
- Mietvertrag
- Aufenthalt
---

# Wohnraumnachweis Aufenthalt

## Definition

Nachweise zum verfügbaren Wohnraum für aufenthaltsrechtliche Verfahren.

## Felder

- Anschrift
- Wohnfläche
- Bewohnerzahl
- Mietverhältnis
- Eigentumsbezug
- Nachweis

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
