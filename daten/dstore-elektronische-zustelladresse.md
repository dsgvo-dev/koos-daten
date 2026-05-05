---
id: dstore-elektronische-zustelladresse
typ: datenspeicher
system: null
name: Elektronische Zustelladresse
datenkategorie: Kontakt & Kommunikation
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: VwVfG
  - gesetz: EGovG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- E-Mail
- Postfach
- Zustellung
---

# Elektronische Zustelladresse

## Definition

Elektronische Adresse für behördliche Kommunikation und Zustellung.

## Felder

- E-Mail-Adresse
- De-Mail oder Postfach
- Einwilligung
- Zustellpräferenz
- Validierungsstatus
- Inhaber/in

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
