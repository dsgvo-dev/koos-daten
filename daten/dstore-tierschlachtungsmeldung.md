---
id: dstore-tierschlachtungsmeldung
typ: datenspeicher
system: null
name: Tierschlachtungsmeldung
datenkategorie: Veterinär & Lebensmittel
zuständige-einheit: oe-amt-71
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: TierSchG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Schlachtung
- Meldung
- Tier
---

# Tierschlachtungsmeldung

## Definition

Meldedaten zu Schlachtungen und zugehörigen veterinärrechtlichen Anforderungen.

## Felder

- Tierart
- Anzahl
- Schlachtort
- Datum
- Verantwortliche Person
- Begleitpapiere

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
