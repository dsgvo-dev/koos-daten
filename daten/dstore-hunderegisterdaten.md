---
id: dstore-hunderegisterdaten
typ: datenspeicher
system: null
name: Hunderegisterdaten
zuständige-einheit: oe-amt-32
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
  - gesetz: NHundG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-12'
tags:
- Hunderegister
- Register
- Hund
---



# Hunderegisterdaten

## Definition

Registerdaten zur Anmeldung eines Hundes im zentralen Hunderegister.

## Felder

- Registernummer
- Chipnummer
- Hundename
- Rasse
- Farbe
- Halterdaten

## Klassifizierung

- Schutzstufe: B
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenspeicher

## Rechtsgrundlagen

- NHundG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Hunderegister
- Einen Hund anmelden

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** Der Bestand wird in einer Gefahrenlage gebraucht, in der es auf Minuten ankommt. Ein Ausfall bedeutet, dass die Kommune die Lage nicht einschätzen kann.

Nach einem Beißvorfall ist die Halterermittlung eilbedürftig.

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** Registernummer, Chipnummer, Hundename, Rasse, Farbe, Halterdaten.

**§ 6 NHundG** verpflichtet die Halterin, bestimmte Daten an ein zentrales Register zu melden. Eine gesetzlich vorgeschriebene Registrierung ohne bewertenden Inhalt.

Die Haltung eines Hundes ist ein nach außen sichtbarer Alltagsvorgang. Für die *gewöhnliche* Hundehaltung trägt keine dieser Datenarten eine Beeinträchtigung der betroffenen Person.

**Abgrenzung.** `dstore-erlaubnis-gefaehrlicher-hund` und `dstore-maulkorb-leinenanordnung` bleiben bei C. Dort belegt der Eintrag einen ordnungsrechtlichen Vorgang gegen die Halterin — die Feststellung der Gefährlichkeit nach § 7 NHundG. Der Unterschied ist nicht der Hund, sondern der Verwaltungsakt.

**`bsi-integritaet` und `bsi-verfuegbarkeit` bleiben hoch.** Im Beißvorfall muss der Halter binnen Minuten ermittelbar sein, und ein verfälschter Registereintrag führt zur falschen Person. Auch hier fallen die beiden Maßstäbe auseinander — für die betroffene Person ist der Eintrag harmlos, für die Gefahrenabwehr ist er tragend.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
