---
id: dstore-loeschwasserversorgung
typ: datenspeicher
system: null
name: Löschwasserversorgung
datenkategorie: Feuerwehr & Brandschutz
zuständige-einheit: oe-amt-37
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: NBauO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Löschwasser
- Brandschutz
---

# Löschwasserversorgung

## Definition

Daten zur gesicherten Löschwasserversorgung eines Standortes oder Vorhabens.

## Felder

- Standort
- Versorgungsart
- Leistung
- Entfernung
- Nachweis
- Stellungnahme

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
