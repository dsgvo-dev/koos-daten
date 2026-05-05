---
id: dstore-lageplan-geobasisdaten
typ: datenspeicher
system: null
name: Lageplan und Geobasisdaten
datenkategorie: Bauen & Grundstück
zuständige-einheit: oe-amt-62
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: NBauO
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Lageplan
- LGLN
- Geobasisdaten
---

# Lageplan und Geobasisdaten

## Definition

Plan- und Kartengrundlagen zur räumlichen Einordnung eines Bauvorhabens.

## Felder

- Lageplan
- Maßstab
- Ausfertigungsdatum
- vermessende Stelle
- Koordinatenbezug
- Grundstücksbezug

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- NBauO

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Baugenehmigung Erteilung
- Genehmigungsfreie Baumaßnahmen Mitteilung
- Antrag auf Verlängerung der Geltungsdauer

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
