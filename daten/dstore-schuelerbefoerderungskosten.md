---
id: dstore-schuelerbefoerderungskosten
typ: datenspeicher
system: null
name: Schülerbeförderungskosten
datenkategorie: Bildung & Schule
zuständige-einheit: oe-amt-40
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: SchulG
  - gesetz: SGB II
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Schülerbeförderung
- Fahrkarte
- Kosten
---

# Schülerbeförderungskosten

## Definition

Kosten- und Nachweisdaten zur Beförderung von Schülerinnen und Schülern.

## Felder

- Schule
- Wegstrecke
- Verkehrsmittel
- Ticketart
- Kosten
- Zeitraum

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
