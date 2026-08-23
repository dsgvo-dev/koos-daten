---
id: dstore-veterinaerrechtliche-betriebsnummer
typ: datenspeicher
system: null
name: Veterinärrechtliche Betriebsnummer
zuständige-einheit: oe-amt-71
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: hoch
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: TierGesG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Betriebsnummer
- Veterinär
- Register
---



# Veterinärrechtliche Betriebsnummer

## Definition

Register- und Kennnummern veterinärrechtlich relevanter Betriebe.

## Felder

- Betriebsnummer
- Betrieb
- Standort
- Tierarten
- Vergabedatum
- Registerstelle

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** Der Bestand wird in einer Gefahrenlage gebraucht, in der es auf Minuten ankommt. Ein Ausfall bedeutet, dass die Kommune die Lage nicht einschätzen kann.

Sie verbindet Betrieb und Tierbestand -- die Schlüsselgröße der Seuchenbekämpfung.

## Schutzstufe geprüft 2026-08-10

**D → B.** **Tiere sind keine betroffenen Personen.** Der gesamte Veterinärbereich stand aus dem Import auf Stufe D, ohne dass eine Angabe über einen Menschen dahinterstünde. Personenbezug besteht allein über die Halterin oder den Betrieb, und dort handelt es sich um gewerbliche Angaben, häufig sogar um eine juristische Person ohne Personenbezug.

Eine Registernummer, die einen Betrieb kennzeichnet -- vergleichbar einer Handelsregisternummer.

**Die BSI-Werte bleiben hoch.** Im Seuchenfall entscheidet die Verfügbarkeit dieser Bestände darüber, wie schnell die Kommune eingrenzen kann. Datenschutz und Informationssicherheit fallen hier auseinander -- das ist kein Widerspruch, sondern der Sinn der getrennten Bewertung.
