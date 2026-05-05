---
id: dstore-verlustanzeige-ausweisdokument
typ: datenspeicher
system: null
name: Verlustanzeige Ausweisdokument
datenkategorie: Identitätsdaten
zuständige-einheit: oe-amt-33
bpmn:
  typ: nachricht
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: PAuswG
  - gesetz: PassG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Verlust
- Ausweis
- Meldung
---

# Verlustanzeige Ausweisdokument

## Definition

Daten zur Anzeige des Verlusts eines Identitätsdokuments gegenüber Behörden.

## Felder

- Dokumentart
- Dokumentnummer
- Verlustdatum
- Verlustort
- betroffene Person
- Meldedatum

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: nachricht

## Rechtsgrundlagen

- PAuswG
- PassG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Verlust des eigenen Personalausweises melden

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
