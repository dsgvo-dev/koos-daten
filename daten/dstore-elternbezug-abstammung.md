---
id: dstore-elternbezug-abstammung
typ: datenspeicher
system: null
name: Elternbezug und Abstammungsangaben
datenkategorie: Personenstandsdaten
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
  - gesetz: BEEG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Eltern
- Abstammung
- Vaterschaft
- Sorgeerklärung
- Sorgeberechtigung
---

# Elternbezug und Abstammungsangaben

## Definition

Daten zur Zuordnung eines Kindes zu Eltern oder Sorgeberechtigten einschließlich Anerkennungs- und Sorgedokumenten.

## Felder

- Vorname Elternteil
- Familienname Elternteil
- Verwandtschaftsverhältnis
- Vaterschaftsanerkennung
- Sorgeerklärung
- Sorgeberechtigung

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- PStG
- PStV
- BEEG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Geburt, Anzeige
- Hausgeburt Anzeige
- Urkunde, Geburtsurkunde/Geburtenregister, Beantragung
- Elterngeld, Antrag

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Familien- und Sorgebezüge wurden nicht in allgemeine Personendaten eingemischt, um sensible Familienverhältnisse klar abzugrenzen.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
