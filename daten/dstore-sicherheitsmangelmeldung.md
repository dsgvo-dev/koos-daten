---
id: dstore-sicherheitsmangelmeldung
typ: datenspeicher
system: null
name: Sicherheitsmangelmeldung
datenkategorie: Ordnung & Sicherheit
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: NPOG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Sicherheitsmangel
- Meldung
- Gefahr
---

# Sicherheitsmangelmeldung

## Definition

Hinweis- oder Meldedaten zu Sicherheitsmängeln im öffentlichen Raum.

## Felder

- Ort
- Mangelbeschreibung
- Gefahrenstufe
- Meldedatum
- Meldende Person
- Bearbeitungsstatus

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
