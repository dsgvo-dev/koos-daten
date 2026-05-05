---
id: dstore-meldeadresse-wohnsitz
typ: datenspeicher
system: null
name: Meldeadresse und Wohnsitzdaten
datenkategorie: Identitätsdaten
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: BMG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Adresse
- Wohnsitz
- Melderegister
- Hauptwohnung
- Nebenwohnung
---

# Meldeadresse und Wohnsitzdaten

## Definition

Daten zur Anschrift, Wohnungszuordnung und melderechtlichen Verknüpfung einer Person.

## Felder

- Straße
- Hausnummer
- Postleitzahl
- Ort
- Hauptwohnung/Nebenwohnung
- Tag des Einzugs
- Tag des Auszugs
- Meldebehörde

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: datenspeicher

## Rechtsgrundlagen

- BMG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Eheschließung, Anmeldung
- Melderegisterauskunft, erweitert, Beantragung
- Personalausweis Beantragung
- Reisepass Beantragung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Aus Meldebescheinigung, Aufenthaltsbescheinigung und Melderegisterauskunft dedupliziert.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
