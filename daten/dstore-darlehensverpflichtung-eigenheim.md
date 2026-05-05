---
id: dstore-darlehensverpflichtung-eigenheim
typ: datenspeicher
system: null
name: Darlehensverpflichtung Eigenheim
datenkategorie: Wohnen & Eigentum
zuständige-einheit: oe-amt-64
bpmn:
  typ: datenspeicher
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
- Darlehen
- Eigenheim
- Belastung
---

# Darlehensverpflichtung Eigenheim

## Definition

Daten zu Darlehen und Kreditverpflichtungen für Kauf, Bau oder Modernisierung eines Eigenheims.

## Felder

- Darlehensgeber
- Darlehenssumme
- Zins
- Tilgung
- Restschuld
- Verwendungszweck

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
