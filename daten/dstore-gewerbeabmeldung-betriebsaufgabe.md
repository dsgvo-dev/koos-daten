---
id: dstore-gewerbeabmeldung-betriebsaufgabe
typ: datenspeicher
system: null
name: Gewerbeabmeldung und Betriebsaufgabe
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
- Abmeldung
- Betriebsaufgabe
---

# Gewerbeabmeldung und Betriebsaufgabe

## Definition

Daten zur Beendigung eines Gewerbebetriebs.

## Felder

- Betrieb
- Betriebsaufgabe am
- Grund
- Ansprechpartner/in
- Aktenzeichen
- Nachweise

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
