---
id: dstore-tierseuchenschutzmeldung
typ: datenspeicher
system: null
name: Tierseuchenschutzmeldung
datenkategorie: Veterinär & Gesundheit
zuständige-einheit: oe-amt-71
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: TierGesG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Tierseuche
- Meldung
- Bestand
---

# Tierseuchenschutzmeldung

## Definition

Meldedaten zu Tierseuchen, Verdachtsfällen oder Schutzmaßnahmen.

## Felder

- Betrieb oder Halter/in
- Tierart
- Meldetatbestand
- Datum
- Bestand
- Maßnahmen

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
