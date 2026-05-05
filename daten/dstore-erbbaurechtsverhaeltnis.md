---
id: dstore-erbbaurechtsverhaeltnis
typ: datenspeicher
system: null
name: Erbbaurechtsverhältnis
datenkategorie: Liegenschaften
zuständige-einheit: oe-amt-23
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: ErbbauRG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Erbbaurecht
- Grundstück
---

# Erbbaurechtsverhältnis

## Definition

Daten zu Erbbaurechten und zugehörigen Vertragsbeziehungen.

## Felder

- Grundstück
- Erbbauberechtigte Person
- Laufzeit
- Erbbauzins
- Vertrag
- Belastungen

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
