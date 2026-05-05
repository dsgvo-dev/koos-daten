---
id: dstore-schulbesuch-ausbildungsstatus
typ: datenspeicher
system: null
name: Schulbesuch und Ausbildungsstatus
datenkategorie: Bildung & Betreuung
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: SGB II
  - gesetz: BKGG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Schule
- Ausbildung
- Teilnahme
---

# Schulbesuch und Ausbildungsstatus

## Definition

Daten zum Schulbesuch oder Ausbildungsstatus von Kindern, Jugendlichen oder jungen Erwachsenen.

## Felder

- Schule oder Ausbildungseinrichtung
- Klassenstufe
- Ausbildungsstatus
- Schulbescheinigung
- Beginn
- Ende

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- SGB II
- BKGG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Bildung und Teilhabe beantragen
- Förderung für Bildung bei jungen Erwachsenen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
