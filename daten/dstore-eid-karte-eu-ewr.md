---
id: dstore-eid-karte-eu-ewr
typ: datenspeicher
system: null
name: eID-Karte EU/EWR
datenkategorie: Identitätsdaten
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: PAuswG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- eID
- EU
- EWR
- Karte
---

# eID-Karte EU/EWR

## Definition

Daten zur eID-Karte für Unionsbürgerinnen und Unionsbürger sowie EWR-Angehörige.

## Felder

- Kartenart
- Inhaber/in
- Gültigkeit
- Ausstellende Behörde
- Sperrkennwort
- Seriennummer

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
