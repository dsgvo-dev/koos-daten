---
id: dstore-unterhaltszahlungen-ansprueche
typ: datenspeicher
system: null
name: Unterhaltszahlungen und Unterhaltsansprüche
datenkategorie: Familie & Soziales
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: BGB
  - gesetz: UVG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Unterhalt
- Anspruch
- Zahlung
---

# Unterhaltszahlungen und Unterhaltsansprüche

## Definition

Daten zu geschuldetem, gezahltem oder erhaltenem Unterhalt.

## Felder

- Unterhaltspflichtige Person
- Berechtigte Person
- Zahlbetrag
- Zeitraum
- Titel oder Vereinbarung
- Zahlungsnachweis

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
