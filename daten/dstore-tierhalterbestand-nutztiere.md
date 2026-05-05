---
id: dstore-tierhalterbestand-nutztiere
typ: datenspeicher
system: null
name: Tierhalterbestand Nutztiere
datenkategorie: Veterinär & Landwirtschaft
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
- Nutztiere
- Bestand
- Halter
---

# Tierhalterbestand Nutztiere

## Definition

Bestandsdaten zu gehaltenen Nutztieren und Haltungsstandorten.

## Felder

- Halter/in
- Betriebsnummer
- Tierarten
- Bestandsgröße
- Standort
- Registerbezug

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
