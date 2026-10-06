---
id: dstore-dienstwagennutzung
bereich: intern
typ: datenspeicher
system: null
name: Dienstwagennutzung
zuständige-einheit: oe-amt-10
personenbezug: ja
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. b und lit. e
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  aufbewahrung:
    frist: 3 Jahre; Fahrtenbuch 1 Jahr
    beginn: nach Ablauf des Kalenderjahres
    hinweis: 'Frist wie in vvt-11-011.'
letzte-aktualisierung: '2026-10-05'
tags:
- Fuhrpark
- Dienstwagen
---

# Dienstwagennutzung

## Definition

Buchung und Nutzung von Pool- und Sonderfahrzeugen durch Beschäftigte.

## Felder

- Name, Vorname, Personalnummer
- Fahrzeug
- Buchungszeitraum
- Fahrtenbuch (Fahrten, Ziele, Kilometer)
- Tankbelege
- Fahrberechtigung

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-11-011 und `proc-dienstwagenbuchung` nutzten bis dahin `dstore-termin-und-vorsprachedaten` und `dstore-fahrzeugnutzungserklaerung` (Kfz-Zulassung), beide extern.

**Schutzstufe C.** Das Fahrtenbuch zeigt Aufenthaltsorte und Bewegungen der Beschäftigten.

**BSI-Vektoren.** Vertraulichkeit normal, Integrität normal, Verfügbarkeit normal — keine besonderen Anforderungen.

**Abgrenzung:**
- `dstore-fahrzeugnutzungserklaerung`: Erklärung im Zulassungsverfahren, extern.
- `dstore-eigenschaden-ksa`: Schäden mit Dienstfahrzeugen.
