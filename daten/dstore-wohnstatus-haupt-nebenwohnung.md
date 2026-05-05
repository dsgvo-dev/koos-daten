---
id: dstore-wohnstatus-haupt-nebenwohnung
typ: datenspeicher
system: null
name: Wohnstatus Haupt- und Nebenwohnung
datenkategorie: Wohnen & Melderecht
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: BMG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Hauptwohnung
- Nebenwohnung
- Wohnstatus
---

# Wohnstatus Haupt- und Nebenwohnung

## Definition

Daten zur Einordnung einer Wohnung als alleinige Wohnung, Hauptwohnung oder Nebenwohnung.

## Felder

- Wohnstatus
- alleinige Wohnung
- Hauptwohnung
- Nebenwohnung
- Wechseldatum

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BMG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Wohnsitz Anmeldung
- Meldebescheinigung Erteilung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
