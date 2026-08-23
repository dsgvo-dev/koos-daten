---
id: dstore-gewerbeanzeige-betriebsstaette
typ: datenspeicher
system: null
name: Gewerbeanzeige und Betriebsstätte
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
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: GewO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-12'
tags:
- Gewerbe
- Betriebsstätte
- Anmeldung
---


# Gewerbeanzeige und Betriebsstätte

## Definition

Grunddaten zur An-, Um- oder Abmeldung eines Gewerbes und zur Betriebsstätte.

## Felder

- Betriebsname
- Betriebsstätte
- Tätigkeit
- Beginn
- Vertretungsberechtigte
- Registerbezug

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Grundlage des Gewerberegisters und der Datenübermittlung an Finanzamt, IHK und Berufsgenossenschaft.

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** Betriebsname, Betriebsstätte, Tätigkeit, Beginn — inhaltsgleich mit der Gewerbeanzeige. Das Gewerberegister ist **kein** öffentliches Register — anders als Handels- und Vereinsregister. Nach § 14 GewO erteilt die Behörde Dritten Auskunft, wenn ein berechtigtes Interesse glaubhaft gemacht wird; die einfache Auskunft beschränkt sich auf Gewerbename, Anschrift und angezeigte Tätigkeit.

Damit scheidet Stufe A aus — frei zugänglich sind die Daten nicht. Ihre Offenbarung beeinträchtigt aber weder die gesellschaftliche Stellung noch die wirtschaftlichen Verhältnisse: Ein angemeldetes Gewerbe wird nach außen betrieben; Firmenschild, Briefkopf und Impressum nennen dieselben Angaben.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
