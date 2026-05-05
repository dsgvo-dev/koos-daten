---
id: dstore-rechnungskorrektur-storno
typ: datenspeicher
system: null
name: Rechnungskorrektur und Storno
datenkategorie: Finanzen & Buchung
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
- Storno
- Korrektur
- Rechnung
---

# Rechnungskorrektur und Storno

## Definition

Daten zu Korrektur-, Gutschrift- oder Stornovorgängen bei Rechnungen.

## Felder

- Ursprungsrechnung
- Korrekturgrund
- Korrekturbetrag
- Datum
- Bezug
- Bearbeitungsstatus

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
