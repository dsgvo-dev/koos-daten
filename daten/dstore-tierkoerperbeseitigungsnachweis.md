---
id: dstore-tierkoerperbeseitigungsnachweis
typ: datenspeicher
system: null
name: Tierkörperbeseitigungsnachweis
datenkategorie: Veterinär & Entsorgung
zuständige-einheit: oe-amt-71
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: TierNebG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Tierkörper
- Beseitigung
- Nachweis
---

# Tierkörperbeseitigungsnachweis

## Definition

Nachweise zur Abholung oder Entsorgung tierischer Nebenprodukte.

## Felder

- Tierart
- Menge
- Abholdatum
- Entsorger
- Herkunftsbetrieb
- Nachweisnummer

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
