---
id: dstore-ordnungswidrigkeitenanzeige
typ: datenspeicher
system: null
name: Ordnungswidrigkeitenanzeige
datenkategorie: Ordnung & Vollzug
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: OWiG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Anzeige
- OWi
- Verstoß
---

# Ordnungswidrigkeitenanzeige

## Definition

Angaben zu einer Anzeige wegen einer Ordnungswidrigkeit.

## Felder

- Anzeigende Person
- Tatort
- Zeitpunkt
- Sachverhalt
- Beweismittel
- Betroffene Person

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
