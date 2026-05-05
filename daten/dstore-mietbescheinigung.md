---
id: dstore-mietbescheinigung
typ: datenspeicher
system: null
name: Mietbescheinigung
datenkategorie: Wohnen & Soziales
zuständige-einheit: oe-amt-64
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: WoGG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Mietbescheinigung
- Vermieter
- Wohnraum
---

# Mietbescheinigung

## Definition

Bescheinigung des Vermieters zu Mietverhältnis, Wohnungsgröße und Nebenkosten.

## Felder

- Vermieter
- Mietobjekt
- Wohnfläche
- Grundmiete
- Nebenkosten
- Einzugsdatum

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
