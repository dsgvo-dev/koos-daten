---
id: dstore-auslaendische-personenstandsurkunde
typ: datenspeicher
system: null
name: Ausländische Personenstandsurkunde
datenkategorie: Auslandsbezug & Dokumente
zuständige-einheit: oe-amt-31
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: PStG
  - gesetz: PStV
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Ausland
- Urkunde
- Personenstand
---

# Ausländische Personenstandsurkunde

## Definition

Ausländische Geburts-, Ehe- oder sonstige Personenstandsurkunden zur Vorlage in deutschen Verfahren.

## Felder

- Urkundenart
- Ausstellungsstaat
- Ausstellungsbehörde
- Ausstellungsdatum
- Registernummer
- Sprache

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- PStG
- PStV

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Geburt im Ausland beurkunden lassen
- Nachbeurkundung einer im Ausland geschlossenen Ehe beantragen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
