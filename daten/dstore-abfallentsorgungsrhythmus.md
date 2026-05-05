---
id: dstore-abfallentsorgungsrhythmus
typ: datenspeicher
system: null
name: Abfallentsorgungsrhythmus
datenkategorie: Umwelt & Entsorgung
zuständige-einheit: oe-amt-60
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: kommunale Satzung
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Abfall
- Rhythmus
- Leerung
---

# Abfallentsorgungsrhythmus

## Definition

Daten zu Entsorgungsintervallen und Behälterleerungen.

## Felder

- Behälter
- Turnus
- Fraktion
- Bereitstellungsort
- Zeitraum
- Status

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
