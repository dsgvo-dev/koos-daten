---
id: dstore-lebensmittelhygienekontrolle
typ: datenspeicher
system: null
name: Lebensmittelhygienekontrolle
datenkategorie: Lebensmittelüberwachung
zuständige-einheit: oe-amt-71
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: LFGB
  - gesetz: VO (EG) 852/2004
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Hygiene
- Kontrolle
- Lebensmittel
---

# Lebensmittelhygienekontrolle

## Definition

Daten zu Hygienekontrollen in Lebensmittelbetrieben.

## Felder

- Betrieb
- Kontrolltermin
- Prüffeld
- Feststellungen
- Mängel
- Auflagen

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
