---
id: dstore-lebensmittelunternehmerdaten
typ: datenspeicher
system: null
name: Lebensmittelunternehmerdaten
datenkategorie: Lebensmittelüberwachung
zuständige-einheit: oe-amt-71
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: LFGB
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Lebensmittelbetrieb
- Unternehmer
---

# Lebensmittelunternehmerdaten

## Definition

Stammdaten von Lebensmittelunternehmern und ihren Betrieben.

## Felder

- Unternehmen
- Betriebsstätte
- Verantwortliche Person
- Tätigkeitsart
- Registrierdatum
- Kontakt

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
