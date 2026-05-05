---
id: dstore-rechnungsadressierung-kommune
typ: datenspeicher
system: null
name: Rechnungsadressierung Kommune
datenkategorie: Finanzen & E-Government
zuständige-einheit: oe-amt-20
bpmn:
  typ: datenspeicher
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
- Adressierung
- Kommune
---

# Rechnungsadressierung Kommune

## Definition

Adressierungsdaten der Kommune für den elektronischen Rechnungsempfang.

## Felder

- Organisationseinheit
- Rechnungsadresse
- E-Mail oder Portal
- Leitweg-ID
- Ansprechpartner/in
- Gültigkeit

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
