---
id: dstore-polizeiliche-verlustmeldung
typ: datenspeicher
system: null
name: Polizeiliche Verlustmeldung
datenkategorie: Sicherheit & Nachweise
zuständige-einheit: oe-amt-33
bpmn:
  typ: nachricht
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: prozessabhängig
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Polizei
- Verlustmeldung
- Anzeige
---

# Polizeiliche Verlustmeldung

## Definition

Nachweis- und Referenzdaten zu einer bei der Polizei aufgenommenen Verlust- oder Diebstahlmeldung.

## Felder

- Dienststelle
- Tagebuchnummer
- Aktenzeichen
- Meldedatum
- Sachverhalt
- betroffenes Dokument

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: nachricht

## Rechtsgrundlagen

- prozessabhängig

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
