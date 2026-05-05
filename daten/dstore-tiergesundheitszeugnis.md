---
id: dstore-tiergesundheitszeugnis
typ: datenspeicher
system: null
name: Tiergesundheitszeugnis
datenkategorie: Veterinär & Gesundheit
zuständige-einheit: oe-amt-71
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: TierGesG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Tiergesundheit
- Zeugnis
- Veterinär
---

# Tiergesundheitszeugnis

## Definition

Gesundheitsbezogener Nachweis für Tiere bei Transport, Handel oder Export.

## Felder

- Tierart
- Tieridentifikation
- Gesundheitsstatus
- Ausstellungsdatum
- Veterinäramt
- Halter/in

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
