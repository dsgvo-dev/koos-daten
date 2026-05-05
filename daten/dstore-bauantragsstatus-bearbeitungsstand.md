---
id: dstore-bauantragsstatus-bearbeitungsstand
typ: datenspeicher
system: null
name: Bauantragsstatus und Bearbeitungsstand
datenkategorie: Bauen & Verfahren
zuständige-einheit: oe-amt-63
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: NBauO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Bauantrag
- Status
- Bearbeitung
---

# Bauantragsstatus und Bearbeitungsstand

## Definition

Status- und Verfahrensdaten zu einem Bauantrag.

## Felder

- Aktenzeichen
- Antragseingang
- Verfahrensstand
- Zuständigkeit
- Fristlauf
- Rückfragen

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
