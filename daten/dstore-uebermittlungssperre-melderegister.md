---
id: dstore-uebermittlungssperre-melderegister
typ: datenspeicher
system: null
name: Übermittlungssperre Melderegister
datenkategorie: Melde- & Schutzdaten
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: BMG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Übermittlungssperre
- Melderegister
- Widerspruch
---

# Übermittlungssperre Melderegister

## Definition

Widerspruchs- und Sperrdaten zur Datenübermittlung aus dem Melderegister.

## Felder

- Betroffene Person
- Sperrart
- Datum des Widerspruchs
- Umfang
- Registervermerk
- Gültigkeit

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
