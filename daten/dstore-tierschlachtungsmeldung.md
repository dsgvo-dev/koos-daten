---
id: dstore-tierschlachtungsmeldung
typ: datenspeicher
system: null
name: Tierschlachtungsmeldung
datenkategorie: Veterinär & Lebensmittel
zuständige-einheit: oe-amt-71
bpmn:
  typ: datenobjekt
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
  - gesetz: TierSchG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Schlachtung
- Meldung
- Tier
---


# Tierschlachtungsmeldung

## Definition

Meldedaten zu Schlachtungen und zugehörigen veterinärrechtlichen Anforderungen.

## Felder

- Tierart
- Anzahl
- Schlachtort
- Datum
- Verantwortliche Person
- Begleitpapiere

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** Der Bestand wird in einer Gefahrenlage gebraucht, in der es auf Minuten ankommt. Ein Ausfall bedeutet, dass die Kommune die Lage nicht einschätzen kann.

Rückverfolgbarkeit in der Lebensmittelkette. Im Seuchenfall muss sie sofort verfügbar sein.

## Schutzstufe geprüft 2026-08-10

**D → B.** **Tiere sind keine betroffenen Personen.** Der gesamte Veterinärbereich stand aus dem Import auf Stufe D, ohne dass eine Angabe über einen Menschen dahinterstünde. Personenbezug besteht allein über die Halterin oder den Betrieb, und dort handelt es sich um gewerbliche Angaben, häufig sogar um eine juristische Person ohne Personenbezug.

Tierart, Anzahl, Schlachtort, Begleitpapiere. Ein Dokument der Rückverfolgbarkeit in der Lebensmittelkette.

**Die BSI-Werte bleiben hoch.** Im Seuchenfall entscheidet die Verfügbarkeit dieser Bestände darüber, wie schnell die Kommune eingrenzen kann. Datenschutz und Informationssicherheit fallen hier auseinander -- das ist kein Widerspruch, sondern der Sinn der getrennten Bewertung.
