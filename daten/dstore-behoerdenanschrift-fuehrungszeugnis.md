---
id: dstore-behoerdenanschrift-fuehrungszeugnis
typ: datenspeicher
system: null
name: Behördenanschrift für Führungszeugnisse
datenkategorie: Sicherheit & Nachweise
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: BZRG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Führungszeugnis
- Behörde
- Anschrift
---

# Behördenanschrift für Führungszeugnisse

## Definition

Adress- und Referenzdaten der Behörde, an die ein behördliches Führungszeugnis übermittelt werden soll.

## Felder

- Behördenname
- Anschrift
- Aktenzeichen
- Verwendungszweck
- Ansprechstelle
- Empfangsweg

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BZRG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Einfaches Führungszeugnis beantragen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
