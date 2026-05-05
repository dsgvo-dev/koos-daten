---
id: dstore-mahn-vollstreckungsstatus
typ: datenspeicher
system: null
name: Mahn- und Vollstreckungsstatus
datenkategorie: Finanzen & Vollstreckung
zuständige-einheit: oe-amt-21
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: VwVG
  - gesetz: AO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Mahnung
- Vollstreckung
- Status
---

# Mahn- und Vollstreckungsstatus

## Definition

Statusdaten zu Mahn- und Vollstreckungsverfahren kommunaler Forderungen.

## Felder

- Forderung
- Mahnstufe
- Vollstreckungsstatus
- Datum
- Zustellungsstatus
- Aktenzeichen

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
