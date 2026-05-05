---
id: dstore-rentenversicherungsverlauf
typ: datenspeicher
system: null
name: Rentenversicherungsverlauf
datenkategorie: Arbeit & Aufenthalt
zuständige-einheit: oe-amt-47
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: SGB VI
  - gesetz: AufenthG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Rente
- Versicherungsverlauf
- Beiträge
---

# Rentenversicherungsverlauf

## Definition

Versicherungs- und Beitragszeiten in der gesetzlichen Rentenversicherung.

## Felder

- Versicherungsnummer
- Beitragszeiten
- Zeitraum
- Rentenversicherungsträger
- Nachweis
- Person

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
