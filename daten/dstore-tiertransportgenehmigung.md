---
id: dstore-tiertransportgenehmigung
typ: datenspeicher
system: null
name: Tiertransportgenehmigung
datenkategorie: Veterinär & Transport
zuständige-einheit: oe-amt-71
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: TierSchTrV
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Tiertransport
- Genehmigung
---

# Tiertransportgenehmigung

## Definition

Genehmigungs- und Nachweisdaten für den gewerblichen Tiertransport.

## Felder

- Antragsteller/in
- Fahrzeug
- Tierarten
- Transportstrecke
- Befähigungsnachweis
- Gültigkeit

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
