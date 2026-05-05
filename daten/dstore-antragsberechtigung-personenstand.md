---
id: dstore-antragsberechtigung-personenstand
typ: datenspeicher
system: null
name: Antragsberechtigung im Personenstandsrecht
datenkategorie: Berechtigungsdaten
zuständige-einheit: oe-amt-31
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: PStG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Berechtigung
- Personenstand
- rechtliches Interesse
---

# Antragsberechtigung im Personenstandsrecht

## Definition

Daten zur Berechtigung, eine Urkunde oder Registerauskunft im Personenstandsrecht zu beantragen.

## Felder

- Rollenbezug
- rechtliches Interesse
- Verwandtschaftsverhältnis
- Nachweisart
- Prüfvermerk
- Entscheidung

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- PStG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Geburtsurkunde beantragen
- Eheurkunde beantragen
- Lebenspartnerschaftsurkunde beantragen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
