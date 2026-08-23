---
id: dstore-schuelerbefoerderungskosten
typ: datenspeicher
system: null
name: Schülerbeförderungskosten
zuständige-einheit: oe-amt-40
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: normal
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: SchulG
  - gesetz: SGB II
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Schülerbeförderung
- Fahrkarte
- Kosten
---


# Schülerbeförderungskosten

## Definition

Kosten- und Nachweisdaten zur Beförderung von Schülerinnen und Schülern.

## Felder

- Schule
- Wegstrecke
- Verkehrsmittel
- Ticketart
- Kosten
- Zeitraum

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-10

**C → D.** Die Leistung wird nur gewährt, wenn die Familie hilfebedürftig ist -- § 28 SGB II, § 34 SGB XII und § 6b BKGG knüpfen sie an den Bezug von Bürgergeld, Sozialhilfe, Wohngeld oder Kinderzuschlag. **Die Datenart offenbart deshalb aus sich heraus den Leistungsbezug einer Familie**, auch wenn kein einziger Betrag darin steht. Das LfD-Schutzstufenkonzept nennt Sozialdaten ausdrücklich als Fall der Stufe D; § 35 SGB I stellt sie unter das Sozialgeheimnis.

Hinzu kommt, wen es trifft: Kinder, deren Bedürftigkeit in Schule, Verein und Mensa für Mitschüler sichtbar werden kann. Genau davor schützt die Einstufung.

Die Beförderung nach § 114 NSchG trifft alle Schülerinnen und Schüler unabhängig vom Einkommen. **Die Datei nennt aber auch SGB II** -- die ergänzende Übernahme nach § 28 Abs. 4 SGB II für Fälle, die die allgemeine Regelung nicht abdeckt. Nach dem Maximalprinzip ist die sensibelste Angabe maßgeblich, die anfallen kann.
