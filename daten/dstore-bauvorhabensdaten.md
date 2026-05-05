---
id: dstore-bauvorhabensdaten
typ: datenspeicher
system: null
name: Bauvorhabens- und Objektdaten
datenkategorie: Bauen & Grundstücke
zuständige-einheit: oe-amt-63
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: NBauO
  - gesetz: NStrG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Bauvorhaben
- Nutzung
- Lageplan
- Werbeanlage
- Gebäude
---

# Bauvorhabens- und Objektdaten

## Definition

Daten zur Beschreibung eines baulichen Vorhabens, seiner Nutzung und der Lage des betroffenen Objekts.

## Felder

- Art des Bauvorhabens
- Nutzungsänderung
- Lageplan
- Gebäudedaten
- Werbeanlage
- Standort des Vorhabens

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- NBauO
- NStrG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Baugenehmigung Erteilung
- Genehmigungsfreie Baumaßnahmen Mitteilung
- Außenwerbung, Genehmigung
- Nutzungsänderung von Gebäuden, Genehmigung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Bau- und Werbeanlagendaten wurden als eigener Sektor abgetrennt, obwohl keine vollständigen Formularfelder offen vorlagen.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
