---
id: dstore-sachkundenachweis-hundehaltung
typ: datenspeicher
system: null
name: Sachkundenachweis Hundehaltung
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: NHundG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-12'
tags:
- Hund
- Sachkunde
- Prüfung
---


# Sachkundenachweis Hundehaltung

## Definition

Nachweis der erforderlichen Sachkunde für die Hundehaltung.

## Felder

- Halter/in
- Prüfungsdatum
- Prüfstelle
- Ergebnis
- Zertifikat
- Hundebezug

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** Halter/in, Prüfungsdatum, Prüfstelle, Ergebnis, Zertifikat.

**§ 3 NHundG** verlangt den Nachweis theoretischer und praktischer Sachkunde, den sogenannten Hundeführerschein. Auch ein negatives Prüfungsergebnis beeinträchtigt die gesellschaftliche Stellung nicht — es hindert lediglich die Anschaffung eines Hundes.

Die Haltung eines Hundes ist ein nach außen sichtbarer Alltagsvorgang. Für die *gewöhnliche* Hundehaltung trägt keine dieser Datenarten eine Beeinträchtigung der betroffenen Person.

**Abgrenzung.** `dstore-erlaubnis-gefaehrlicher-hund` und `dstore-maulkorb-leinenanordnung` bleiben bei C. Dort belegt der Eintrag einen ordnungsrechtlichen Vorgang gegen die Halterin — die Feststellung der Gefährlichkeit nach § 7 NHundG. Der Unterschied ist nicht der Hund, sondern der Verwaltungsakt.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
