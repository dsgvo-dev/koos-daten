---
id: dstore-grundsteuerbescheid-eigentum
typ: datenspeicher
system: null
name: Grundsteuerbescheid Eigentum
datenkategorie: Steuern & Eigentum
zuständige-einheit: oe-amt-22
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: GrStG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Grundsteuer
- Bescheid
- Eigentum
---

# Grundsteuerbescheid Eigentum

## Definition

Bescheiddaten zur Grundsteuer für selbst genutztes oder vermietetes Wohneigentum.

## Felder

- Steuerobjekt
- Aktenzeichen
- Steuerjahr
- Festgesetzter Betrag
- Fälligkeit
- Eigentümer

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
