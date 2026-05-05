---
id: dstore-gewerbeanzeige-betriebsstaette
typ: datenspeicher
system: null
name: Gewerbeanzeige und Betriebsstätte
datenkategorie: Gewerbe & Betrieb
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: GewO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Gewerbe
- Betriebsstätte
- Anmeldung
---

# Gewerbeanzeige und Betriebsstätte

## Definition

Grunddaten zur An-, Um- oder Abmeldung eines Gewerbes und zur Betriebsstätte.

## Felder

- Betriebsname
- Betriebsstätte
- Tätigkeit
- Beginn
- Vertretungsberechtigte
- Registerbezug

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
