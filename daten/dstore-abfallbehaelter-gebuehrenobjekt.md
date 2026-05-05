---
id: dstore-abfallbehaelter-gebuehrenobjekt
typ: datenspeicher
system: null
name: Abfallbehälter und Gebührenobjekt
datenkategorie: Umwelt & Gebühren
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
- Behälter
- Gebühr
---

# Abfallbehälter und Gebührenobjekt

## Definition

Daten zu Abfallbehältern, Anschlussobjekten und Gebührenpflicht.

## Felder

- Objektadresse
- Behälterart
- Volumen
- Leerungsrhythmus
- Gebührenpflichtige Person
- Startdatum

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
