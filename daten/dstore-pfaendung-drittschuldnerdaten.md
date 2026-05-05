---
id: dstore-pfaendung-drittschuldnerdaten
typ: datenspeicher
system: null
name: Pfändungs- und Drittschuldnerdaten
datenkategorie: Finanzen & Vollstreckung
zuständige-einheit: oe-amt-21
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: ZPO
  - gesetz: VwVG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Pfändung
- Drittschuldner
---

# Pfändungs- und Drittschuldnerdaten

## Definition

Daten zu Pfändungen und beteiligten Drittschuldnern.

## Felder

- Schuldner/in
- Drittschuldner
- Forderungsart
- Pfändungsbetrag
- Verfügung
- Zustellung

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
