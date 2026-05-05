---
id: dstore-haushaltsbescheinigung
typ: datenspeicher
system: null
name: Haushaltsbescheinigung
datenkategorie: Wohnen & Soziales
zuständige-einheit: oe-amt-50
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
- Haushalt
- Bescheinigung
- Mitglieder
---

# Haushaltsbescheinigung

## Definition

Behördliche Bescheinigung über die Zusammensetzung eines Haushalts.

## Felder

- Haushaltsvorstand
- Haushaltsmitglieder
- Anschrift
- Ausstellungsdatum
- Ausstellende Stelle
- Gültigkeitsbezug

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
