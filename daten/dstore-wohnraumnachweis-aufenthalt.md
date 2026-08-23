---
id: dstore-wohnraumnachweis-aufenthalt
typ: datenspeicher
system: null
name: Wohnraumnachweis Aufenthalt
zuständige-einheit: oe-amt-47
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: AufenthG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-04'
tags:
- Wohnraum
- Mietvertrag
- Aufenthalt
---


# Wohnraumnachweis Aufenthalt

## Definition

Nachweise zum verfügbaren Wohnraum für aufenthaltsrechtliche Verfahren.

## Felder

- Anschrift
- Wohnfläche
- Bewohnerzahl
- Mietverhältnis
- Eigentumsbezug
- Nachweis

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-14

**C → D.** Die Zugehörigkeit zum Speicher offenbart das Aufenthaltsverfahren — ein
Wohnraumnachweis *für aufenthaltsrechtliche Verfahren* wird nicht neutral geführt. Genutzt in
`vvt-47-006` und `vvt-50-005` (beide vertraulich). Dieselbe Logik wie
`dstore-termin-und-vorsprachedaten` (D). Die BSI-Vertraulichkeit folgt auf `hoch`.
