---
id: dstore-stiftungsleistung
bereich: extern
typ: datenspeicher
system: null
name: Stiftungsleistung
zuständige-einheit: oe-amt-20
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
    artikel: § 3
  - gesetz: NStiftG
    artikel: Niedersächsisches Stiftungsgesetz
  - gesetz: AO
    artikel: § 147
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Ablauf des Jahres der Auszahlung
    hinweis: 'Frist wie in vvt-20-007 (Abgabenordnung).'
letzte-aktualisierung: '2026-10-05'
tags:
- Stiftung
- Zuwendung
---

# Stiftungsleistung

## Definition

Leistungen kommunaler Stiftungen an Empfängerinnen und Empfänger nach dem Stiftungszweck.

## Felder

- Empfängerin oder Empfänger
- Stiftungszweck und Bewilligungsgrund
- Höhe der Zuwendung
- Auszahlung und Bankverbindung
- Verwendungsnachweis

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-20-007 nutzte bis dahin `dstore-debitoren-kreditorendaten` (Kasse, intern).

**Schutzstufe C.** Angaben zur Bedürftigkeit können je nach Stiftungszweck anfallen.

**BSI-Vektoren.** Vertraulichkeit normal, Integrität normal, Verfügbarkeit normal — keine besonderen Anforderungen.

**Abgrenzung:**
- `dstore-spende-zuwendung`: Spenden an die Kommune, nicht Leistungen der Stiftung.
- `dstore-debitoren-kreditorendaten`: Buchung bei der Kasse, intern.
