---
id: dstore-erschliessungsbeitragsdaten
typ: datenspeicher
system: null
name: Erschließungsbeitragsdaten
datenkategorie: Bauen & Beiträge
zuständige-einheit: oe-amt-22
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: BauGB
  - gesetz: NKAG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Erschließung
- Beitrag
---

# Erschließungsbeitragsdaten

## Definition

Daten zur Erhebung von Erschließungsbeiträgen.

## Felder

- Grundstück
- Maßnahme
- Beitragspflichtige Person
- Verteilungsmaßstab
- Bescheid
- Fälligkeit

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
