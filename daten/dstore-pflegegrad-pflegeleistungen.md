---
id: dstore-pflegegrad-pflegeleistungen
typ: datenspeicher
system: null
name: Pflegegrad und Pflegeleistungen
datenkategorie: Soziales & Gesundheit
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: SGB XI
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Pflegegrad
- Pflegeversicherung
- Leistung
---

# Pflegegrad und Pflegeleistungen

## Definition

Angaben zu anerkanntem Pflegegrad und bewilligten Pflegeleistungen.

## Felder

- Pflegegrad
- Leistungsart
- Bewilligungszeitraum
- Pflegekasse
- Bescheid
- Pflegebedürftige Person

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
