---
id: dstore-gewerbeabmeldung-betriebsaufgabe
typ: datenspeicher
system: null
name: Gewerbeabmeldung und Betriebsaufgabe
datenkategorie: Gewerbe & Betrieb
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
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
- Abmeldung
- Betriebsaufgabe
---


# Gewerbeabmeldung und Betriebsaufgabe

## Definition

Daten zur Beendigung eines Gewerbebetriebs.

## Felder

- Betrieb
- Betriebsaufgabe am
- Grund
- Ansprechpartner/in
- Aktenzeichen
- Nachweise

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Eine unterbliebene oder verfälschte Abmeldung führt zu Beitrags- und Steuerforderungen gegen eine Person, die kein Gewerbe mehr betreibt.

## Schutzstufe geprüft 2026-08-12

**Bleibt bei C** — als einziger Gewerbespeicher dieses Loses.

Anders als An- und Ummeldung führt dieser Speicher das Feld **„Grund"** der Betriebsaufgabe. Der Grund kann Insolvenz, Krankheit oder Geschäftsaufgabe wegen Erfolglosigkeit sein. Das betrifft die wirtschaftlichen Verhältnisse und damit das Kriterium der Stufe C.

**Abgrenzung.** `dstore-gewerbedaten`, `dstore-gewerbeanzeige-betriebsstaette` und `dstore-gewerbeummeldung-aenderungsdaten` sind am 2026-08-12 auf B herabgestuft worden. Der Unterschied ist dieses eine Feld.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
