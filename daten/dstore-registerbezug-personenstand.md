---
id: dstore-registerbezug-personenstand
typ: datenspeicher
system: null
name: Registerbezug Personenstand
datenkategorie: Register- und Nachweisdaten
zuständige-einheit: oe-amt-31
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: PStG
  - gesetz: PStV
  aufbewahrung:
    frist: 110/80/30 Jahre je Registerart
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Standesamt
- Geburtenregister
- Eheregister
- Sterberegister
- Registerauszug
---

# Registerbezug Personenstand

## Definition

Daten zur Identifikation und Auswertung von Einträgen in Personenstandsregistern.

## Felder

- Registerart
- zuständiges Standesamt
- Beurkundungsnummer
- Registerjahr
- Registerauszug
- Registerbehörde

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenspeicher

## Rechtsgrundlagen

- PStG
- PStV

## Aufbewahrung

- Frist: 110/80/30 Jahre je Registerart
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Urkunde, Geburtsurkunde/Geburtenregister, Beantragung
- Urkunde, Eheurkunde, Beantragung
- Personenstandsauskünfte
- Sterbefall im Ausland

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Die Fristen spiegeln die im Portal genannten Registerfristen wider: Geburt 110, Ehe/Lebenspartnerschaft 80, Sterbeeinträge 30 Jahre.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
