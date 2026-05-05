---
id: dstore-baulastenauszug
typ: datenspeicher
system: null
name: Baulastenauszug
datenkategorie: Bauen & Grundstück
zuständige-einheit: oe-amt-63
bpmn:
  typ: datenobjekt
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
- Baulast
- Auszug
- Grundstück
---

# Baulastenauszug

## Definition

Auszugsdaten aus dem Baulastenverzeichnis.

## Felder

- Grundstück
- Baulastart
- Eintragungsdatum
- Inhalt
- Aktenzeichen
- Auskunftsempfänger/in

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
