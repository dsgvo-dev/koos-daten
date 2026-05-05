---
id: dstore-gaststaettenbetrieb-anzeigedaten
typ: datenspeicher
system: null
name: Gaststättenbetrieb Anzeigedaten
datenkategorie: Gewerbe & Gastronomie
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: GastG
  - gesetz: GewO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Gaststätte
- Betrieb
- Anzeige
---

# Gaststättenbetrieb Anzeigedaten

## Definition

Anzeige- und Grunddaten eines Gaststättenbetriebs.

## Felder

- Betriebsart
- Betreiber/in
- Anschrift
- Öffnungszeiten
- Verantwortliche Person
- Anzeigezeitpunkt

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
