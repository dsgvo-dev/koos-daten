---
id: dstore-auskunftssperre-melderegister
typ: datenspeicher
system: null
name: Auskunftssperre Melderegister
datenkategorie: Melde- & Schutzdaten
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: BMG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Auskunftssperre
- Melderegister
- Schutz
---

# Auskunftssperre Melderegister

## Definition

Sperrvermerk zum Schutz gefährdeter Personen im Melderegister.

## Felder

- Betroffene Person
- Sperrgrund
- Anordnende Behörde
- Gültigkeitszeitraum
- Prüffrist
- Aktenbezug

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
