---
id: dstore-flur-flurstueck-lagebezeichnung
typ: datenspeicher
system: null
name: Flur, Flurstück und Lagebezeichnung
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
  - gesetz: Vermessungsrecht
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Flur
- Flurstück
- Lagebezeichnung
---

# Flur, Flurstück und Lagebezeichnung

## Definition

Katasterbezogene Identifikationsdaten eines Grundstücks.

## Felder

- Gemarkung
- Flur
- Flurstück
- Lagebezeichnung
- Katasteramt
- Nachweisdatum

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- NBauO
- Vermessungsrecht

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Baugenehmigung Erteilung
- Genehmigungsfreie Baumaßnahmen Mitteilung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
