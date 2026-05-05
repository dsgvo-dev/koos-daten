---
id: dstore-ausnahmegenehmigung-schwerverkehr
typ: datenspeicher
system: null
name: Ausnahmegenehmigung Schwerverkehr
datenkategorie: Verkehr & Genehmigungen
zuständige-einheit: oe-amt-34
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: StVO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Ausnahmegenehmigung
- Schwerverkehr
---

# Ausnahmegenehmigung Schwerverkehr

## Definition

Genehmigungsdaten für Ausnahmen vom Verkehrsrecht bei Schwer- oder Großraumverkehr.

## Felder

- Antragsteller/in
- Anlass
- Streckenbezug
- Auflagen
- Geltungsdauer
- Bescheid

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
