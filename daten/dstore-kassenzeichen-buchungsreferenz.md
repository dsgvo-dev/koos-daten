---
id: dstore-kassenzeichen-buchungsreferenz
typ: datenspeicher
system: null
name: Kassenzeichen und Buchungsreferenz
datenkategorie: Finanzen & Zahlung
zuständige-einheit: oe-amt-20
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: KomHKVO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Kassenzeichen
- Buchung
---

# Kassenzeichen und Buchungsreferenz

## Definition

Referenzkennzeichen zur Zuordnung von Forderungen und Zahlungen.

## Felder

- Kassenzeichen
- Buchungsreferenz
- Forderungsart
- Betrag
- Fälligkeit
- Schuldner/in

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
