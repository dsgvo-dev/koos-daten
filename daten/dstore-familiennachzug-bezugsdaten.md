---
id: dstore-familiennachzug-bezugsdaten
typ: datenspeicher
system: null
name: Familiennachzugbezug
datenkategorie: Migration & Familie
zuständige-einheit: oe-amt-47
bpmn:
  typ: datenspeicher
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
letzte-aktualisierung: '2026-08-10'
tags:
- Familiennachzug
- Ehe
- Kind
---


# Familiennachzugbezug

## Definition

Daten zum familiären Bezug im Rahmen des Familiennachzugs.

## Felder

- Bezugsperson
- Familienverhältnis
- Aufenthaltstitel Bezugsperson
- Wohnraum
- Lebensunterhalt
- Nachweise

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-10

**C → D.** **An dieser Datenart hängt, ob eine Familie zusammenleben darf.** Sie führt das Familienverhältnis, den Aufenthaltstitel der Bezugsperson, den Wohnraum und die Sicherung des Lebensunterhalts zusammen -- also die Prüfung nach §§ 27 ff. AufenthG in ihrer Gesamtheit.

Der Aufenthaltstitel der Bezugsperson lässt die Herkunft erkennen und, bei einem Titel nach § 25 Abs. 1 oder 2 AufenthG, die Anerkennung als Asylberechtigte oder Flüchtling -- eine Angabe, deren Offenlegung gegenüber dem Herkunftsstaat Menschen gefährden kann. Die Prüfung des Lebensunterhalts fügt die wirtschaftlichen Verhältnisse hinzu.
