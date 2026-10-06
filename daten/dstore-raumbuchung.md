---
id: dstore-raumbuchung
bereich: intern
typ: datenspeicher
system: null
name: Raumbuchung
zuständige-einheit: oe-amt-10
personenbezug: ja
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. e
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  aufbewahrung:
    frist: 1 Jahr
    beginn: nach dem Nutzungstermin
    hinweis: 'Frist wie in vvt-15-006.'
letzte-aktualisierung: '2026-10-05'
tags:
- Raumbuchung
- Organisation
---

# Raumbuchung

## Definition

Buchungen von Sitzungszimmern und Besprechungsräumen durch Beschäftigte.

## Felder

- buchende Person und dienstliche Kontaktdaten
- Raum
- Datum und Uhrzeit
- Teilnehmerzahl
- gewünschte Ausstattung
- Buchungsbestätigung

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-15-006 und `proc-raumbuchung` nutzten bis dahin `dstore-termin-und-vorsprachedaten` (Bürgertermine) und `dstore-kontaktdaten`, beide extern.

**Schutzstufe B.** Dienstliche Angaben.

**BSI-Vektoren.** Vertraulichkeit normal, Integrität normal, Verfügbarkeit normal — keine besonderen Anforderungen.

**Abgrenzung:**
- `dstore-termin-und-vorsprachedaten`: Termine von Bürgerinnen und Bürgern, extern.
