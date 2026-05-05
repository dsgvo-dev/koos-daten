---
id: dstore-hundehaltung
typ: datenspeicher
system: null
name: Hundehaltung
datenkategorie: Tiere & Haltung
zuständige-einheit: oe-amt-32
bpmn:
  typ: nachricht
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: NHundG
  - gesetz: kommunale Satzung
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Hund
- Haltung
- Anmeldung
---

# Hundehaltung

## Definition

Grunddaten zur Haltung eines Hundes im Gemeindegebiet.

## Felder

- Halterin oder Halter
- Beginn Hundehaltung
- Hundename
- Rasse
- Geburtsdatum Hund
- Haltungsanschrift

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: nachricht

## Rechtsgrundlagen

- NHundG
- kommunale Satzung

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Hundehaltung Anmeldung
- Einen Hund anmelden
- Hundehaltung Abmeldung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
