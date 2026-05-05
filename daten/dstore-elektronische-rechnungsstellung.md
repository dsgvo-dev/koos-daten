---
id: dstore-elektronische-rechnungsstellung
typ: datenspeicher
system: null
name: Elektronische Rechnungsstellung
datenkategorie: Finanzen & E-Government
zuständige-einheit: oe-amt-20
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: ERechV
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Rechnung
- Elektronisch
- XRechnung
---

# Elektronische Rechnungsstellung

## Definition

Strukturierte Daten einer elektronischen Rechnung an die Kommune.

## Felder

- Rechnungsnummer
- Rechnungsdatum
- Leitweg-ID
- Betrag
- Leistungsempfänger
- Format

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
