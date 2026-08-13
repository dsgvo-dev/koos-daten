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
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: PStG
  - gesetz: PStV
  aufbewahrung:
    frist: 110/80/30 Jahre je Registerart
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-10'
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

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** An den Vorgang knüpft eine gesetzliche Frist. Ist der Bestand im entscheidenden Zeitraum nicht abrufbar, läuft die Frist gleichwohl -- mit Rechtsfolgen für die Kommune oder die betroffene Person.

Der Registerbezug ist Voraussetzung für jede Urkundenausstellung.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Familiäre, aufenthaltsrechtliche und weltanschauliche Verhältnisse.** Anders als bei den am selben Tag herabgestuften Personenstandsspeichern trägt dieser Bestand eine Angabe, die für sich genommen belastend ist -- eine Sorgerechtsentscheidung, die Abstammung, die Religionszugehörigkeit, den Aufenthaltsstatus oder die Ausübung eines Grundrechts. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
