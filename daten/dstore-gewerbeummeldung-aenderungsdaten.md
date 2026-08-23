---
id: dstore-gewerbeummeldung-aenderungsdaten
typ: datenspeicher
system: null
name: Gewerbeummeldung Änderungsdaten
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
- Änderung
- Ummeldung
---


# Gewerbeummeldung Änderungsdaten

## Definition

Änderungsdaten bei Verlegung, Erweiterung oder Wechsel der Tätigkeit eines Gewerbes.

## Felder

- Bisherige Daten
- Neue Daten
- Wirksamkeitsdatum
- Grund der Änderung
- Ansprechpartner/in
- Nachweise

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Wie bei An- und Abmeldung: Der Registerstand muss stimmen.

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** Verlegung, Erweiterung oder Wechsel der Tätigkeit. Das Gewerberegister ist **kein** öffentliches Register — anders als Handels- und Vereinsregister. Nach § 14 GewO erteilt die Behörde Dritten Auskunft, wenn ein berechtigtes Interesse glaubhaft gemacht wird; die einfache Auskunft beschränkt sich auf Gewerbename, Anschrift und angezeigte Tätigkeit.

Damit scheidet Stufe A aus — frei zugänglich sind die Daten nicht. Ihre Offenbarung beeinträchtigt aber weder die gesellschaftliche Stellung noch die wirtschaftlichen Verhältnisse: Ein angemeldetes Gewerbe wird nach außen betrieben; Firmenschild, Briefkopf und Impressum nennen dieselben Angaben.

**Abgrenzung zur Abmeldung.** `dstore-gewerbeabmeldung-betriebsaufgabe` bleibt bei C, weil es den *Grund* der Betriebsaufgabe führt — der kann Insolvenz sein. Das Feld „Grund der Änderung" bei der Ummeldung trägt das nicht: Es nennt eine unternehmerische Entscheidung, keine Notlage.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
