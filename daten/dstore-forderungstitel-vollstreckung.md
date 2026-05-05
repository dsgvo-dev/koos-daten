---
id: dstore-forderungstitel-vollstreckung
typ: datenspeicher
system: null
name: Forderungstitel Vollstreckung
datenkategorie: Finanzen & Vollstreckung
zuständige-einheit: oe-amt-21
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: ZPO
  - gesetz: VwVG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Titel
- Vollstreckung
- Forderung
---

# Forderungstitel Vollstreckung

## Definition

Daten zu vollstreckbaren Forderungstiteln.

## Felder

- Titelart
- Aktenzeichen
- Schuldner/in
- Forderungsbetrag
- Erlassdatum
- Vollstreckbarkeit

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
