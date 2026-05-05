---
id: dstore-vergabe-auftragsbezug
typ: datenspeicher
system: null
name: Vergabe- und Auftragsbezug
datenkategorie: Beschaffung & Finanzen
zuständige-einheit: oe-amt-10
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: VgV
  - gesetz: UVgO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Vergabe
- Auftrag
- Leistung
---

# Vergabe- und Auftragsbezug

## Definition

Daten zum Bezug einer Rechnung oder Zahlung auf Vergabe- und Auftragsvorgänge.

## Felder

- Vergabenummer
- Auftragnehmer/in
- Leistungsbeschreibung
- Bestelldatum
- Auftragswert
- Rechnungsbezug

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
