---
id: dstore-einbuergerungszusicherung
typ: datenspeicher
system: null
name: Einbürgerungszusicherung
datenkategorie: Migration & Einbürgerung
zuständige-einheit: oe-amt-47
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: StAG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Einbürgerung
- Zusicherung
---

# Einbürgerungszusicherung

## Definition

Zusicherungs- und Verfahrensdaten einer beabsichtigten Einbürgerung.

## Felder

- Aktenzeichen
- Zusicherungsdatum
- Voraussetzungen
- Aufgabe bisheriger Staatsangehörigkeit
- Person
- Gültigkeit

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
