---
id: dstore-tierhalterbestand-nutztiere
typ: datenspeicher
system: null
name: Tierhalterbestand Nutztiere
datenkategorie: Veterinär & Landwirtschaft
zuständige-einheit: oe-amt-71
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
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
- Nutztiere
- Bestand
- Halter
---


# Tierhalterbestand Nutztiere

## Definition

Bestandsdaten zu gehaltenen Nutztieren und Haltungsstandorten.

## Felder

- Halter/in
- Betriebsnummer
- Tierarten
- Bestandsgröße
- Standort
- Registerbezug

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit hoch.** Der Bestand dient der Gefahrenabwehr. Ist er verfälscht oder im entscheidenden Moment nicht abrufbar, kann die Kommune ihre Schutzaufgabe nicht erfüllen -- mit möglichen Folgen für Leib und Leben.

Der Bestand ist Grundlage der Rückverfolgbarkeit im Tierseuchenfall. Verfälschte Bestandszahlen verhindern die Eingrenzung eines Ausbruchs.

## Schutzstufe geprüft 2026-08-10

**D → C.** **Tiere sind keine betroffenen Personen.** Der gesamte Veterinärbereich stand aus dem Import auf Stufe D, ohne dass eine Angabe über einen Menschen dahinterstünde. Personenbezug besteht allein über die Halterin oder den Betrieb, und dort handelt es sich um gewerbliche Angaben, häufig sogar um eine juristische Person ohne Personenbezug.

**Ein Umstand hält diesen Speicher über den übrigen:** Die Bestandsgröße ist bei einem landwirtschaftlichen Einzelunternehmen zugleich eine Angabe über das Betriebsvermögen und damit über die wirtschaftlichen Verhältnisse der Halterin oder des Halters -- Betrieb und Person fallen dort zusammen. Stufe C, nicht B.
