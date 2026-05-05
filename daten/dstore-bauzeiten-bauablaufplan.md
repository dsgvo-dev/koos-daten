---
id: dstore-bauzeiten-bauablaufplan
typ: datenspeicher
system: null
name: Bauzeiten- und Bauablaufplan
datenkategorie: Bauen & Organisation
zuständige-einheit: oe-amt-63
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: NBauO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Bauzeit
- Ablaufplan
---

# Bauzeiten- und Bauablaufplan

## Definition

Zeit- und Ablaufplanung eines Bauvorhabens.

## Felder

- Bauabschnitt
- Beginn
- Ende
- Gewerke
- Verantwortliche Person
- Meilensteine

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
