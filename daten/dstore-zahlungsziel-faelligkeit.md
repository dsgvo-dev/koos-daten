---
id: dstore-zahlungsziel-faelligkeit
typ: datenspeicher
system: null
name: Zahlungsziel und Fälligkeit
datenkategorie: Finanzen & Zahlung
zuständige-einheit: oe-amt-20
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: BGB
  - gesetz: KomHKVO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Fälligkeit
- Zahlungsziel
---

# Zahlungsziel und Fälligkeit

## Definition

Daten zu Fälligkeiten, Zahlungszielen und Skontoregelungen.

## Felder

- Fälligkeit
- Zahlungsziel
- Skonto
- Bezugsvorgang
- Betrag
- Status

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
