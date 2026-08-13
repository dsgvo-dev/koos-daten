---
id: dstore-lebensmittelhygienekontrolle
typ: datenspeicher
system: null
name: Lebensmittelhygienekontrolle
datenkategorie: Lebensmittelüberwachung
zuständige-einheit: oe-amt-71
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
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: LFGB
  - gesetz: VO (EG) 852/2004
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-04'
tags:
- Hygiene
- Kontrolle
- Lebensmittel
---


# Lebensmittelhygienekontrolle

## Definition

Daten zu Hygienekontrollen in Lebensmittelbetrieben.

## Felder

- Betrieb
- Kontrolltermin
- Prüffeld
- Feststellungen
- Mängel
- Auflagen

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** Der Bestand wird in einer Gefahrenlage gebraucht, in der es auf Minuten ankommt. Ein Ausfall bedeutet, dass die Kommune die Lage nicht einschätzen kann.

Bei einem Rückruf oder Ausbruchsgeschehen entscheidet die Geschwindigkeit über den Schaden.
