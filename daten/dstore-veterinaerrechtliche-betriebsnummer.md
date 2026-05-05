---
id: dstore-veterinaerrechtliche-betriebsnummer
typ: datenspeicher
system: null
name: Veterinärrechtliche Betriebsnummer
datenkategorie: Veterinär & Register
zuständige-einheit: oe-amt-71
bpmn:
  typ: datenspeicher
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
- Betriebsnummer
- Veterinär
- Register
---

# Veterinärrechtliche Betriebsnummer

## Definition

Register- und Kennnummern veterinärrechtlich relevanter Betriebe.

## Felder

- Betriebsnummer
- Betrieb
- Standort
- Tierarten
- Vergabedatum
- Registerstelle

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
