---
id: dstore-meldeadresse-wohnsitz
typ: datenspeicher
system: null
name: Meldeadresse und Wohnsitzdaten
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: BMG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-12'
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

- Schutzstufe: B
- Schutzbedarf: normal
- Vertraulichkeit: intern
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

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** Der Speicher wird in so vielen Verfahren geführt, dass ein Ausfall nicht ein Verfahren verzögert, sondern den Publikumsverkehr insgesamt zum Erliegen bringt. Das ist der Maßstab des BSI: erhebliche Beeinträchtigung der Aufgabenerfüllung.

15 Verwendungen. Die Anschrift ist Voraussetzung nahezu jeder Zustellung und jedes Bescheids.

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** Die einfache Melderegisterauskunft nach **§ 44 BMG** gibt Familienname, Vornamen, Doktorgrad und die derzeitige Anschrift an jedermann heraus — ohne dass ein berechtigtes Interesse darzulegen wäre. Erst die erweiterte Auskunft nach § 45 BMG verlangt eines.

Die derzeitige Anschrift ist damit ein Datum, das die Meldebehörde am Schalter jedem
Anfragenden herausgibt. Eine Schutzstufe C dafür verlangt Maßnahmen für etwas, das die
Behörde von Gesetzes wegen offenlegt.

`dstore-adresse` steht seit dem 2026-08-10 aus demselben Grund auf B. Zwei Speicher mit
demselben Inhalt können nicht verschieden eingestuft sein.

**Die Ausnahme regelt das Melderecht selbst, und der Bestand bildet sie ab:** die
Auskunftssperre nach § 51 BMG in `dstore-auskunftssperre-melderegister` (Stufe E), der
bedingte Sperrvermerk nach § 52 BMG in `dstore-schutzbeduerftigkeitskennzeichen` (Stufe E)
und die vertraulichen Verfahren in `dstore-adresse-vertraulich` (Stufe D). Die Anschrift ist
nicht deshalb hoch einzustufen, weil sie im Einzelfall gefährlich ist — dafür stehen drei
eigene Speicher bereit, zwei davon auf E.

**Wirksamster Posten des Loses:** 15 Verwendungen in sechs Ämtern.

*Durchsicht Los 2 (Amt 33) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los2-amt33.md`.*
