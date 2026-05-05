---
id: dstore-personenstammdaten
typ: datenspeicher
system: null
name: Personenstammdaten
datenkategorie: Identitätsdaten
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: PStG
  - gesetz: PStV
  - gesetz: BMG
  - gesetz: PAuswG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Name
- Vorname
- Geburtsdatum
- Geburtsort
- Geschlecht
- Doktorgrad
---

# Personenstammdaten

## Definition

Grundlegende Identifikations- und Zuordnungsdaten natürlicher Personen, wie sie in Personenstands-, Melde- und Ausweisverfahren wiederkehrend verarbeitet werden.

## Felder

- Vorname
- Familienname
- frühere Namen
- Geburtsdatum
- Geburtsort
- Geschlecht
- Doktorgrad

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- PStG
- PStV
- BMG
- PAuswG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Urkunde, Geburtsurkunde/Geburtenregister, Beantragung
- Eheschließung, Anmeldung
- Geburt, Anzeige
- Melderegisterauskunft, erweitert, Beantragung
- Personalausweis Beantragung
- Reisepass Beantragung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Zusammengeführt aus Personenstands-, Melde- und Identitätsverfahren; zentrale Basiskategorie ohne Spezialnachweise.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
