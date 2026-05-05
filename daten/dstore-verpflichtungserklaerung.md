---
id: dstore-verpflichtungserklaerung
typ: datenspeicher
system: null
name: Verpflichtungserklärung
datenkategorie: Migration & Verpflichtung
zuständige-einheit: oe-amt-47
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: AufenthG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Verpflichtung
- Besucher
- Unterhalt
---

# Verpflichtungserklärung

## Definition

Erklärung zur Übernahme von Lebensunterhalts- und Ausreisekosten für Dritte.

## Felder

- Verpflichtungsgeber
- Begünstigte Person
- Bonitätsnachweis
- Zeitraum
- Anlass
- Aktenzeichen

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
