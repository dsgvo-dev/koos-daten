---
id: dstore-heilpraktikererlaubnisverfahren
typ: datenspeicher
system: null
name: Heilpraktikererlaubnisverfahren
datenkategorie: Gesundheit & Erlaubnisse
zuständige-einheit: oe-amt-53
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: HeilprG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Heilpraktiker
- Erlaubnis
- Prüfung
---

# Heilpraktikererlaubnisverfahren

## Definition

Antrags- und Prüfdaten für die Erteilung einer Heilpraktikererlaubnis.

## Felder

- Antragstellende Person
- Fachgebiet
- Prüfungsdatum
- Gesundheitszeugnis
- Führungszeugnis
- Erlaubnisstatus

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
