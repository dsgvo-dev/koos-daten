---
id: dstore-kehrbezirk-bestellung
typ: datenspeicher
system: null
name: Kehrbezirk und Bestellung Bezirksschornsteinfeger
datenkategorie: Gewerbe & Erlaubnisse
zuständige-einheit: oe-amt-60
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
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: SchfHwG
    artikel: § 5
  - gesetz: SchfHwG
    artikel: § 8
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Ende der Bestellung
letzte-aktualisierung: '2026-08-10'
tags:
- Schornsteinfeger
- Kehrbezirk
---


# Kehrbezirk und Bestellung Bezirksschornsteinfeger

## Definition

Bestellung bevollmächtigter Bezirksschornsteinfegerinnen und -schornsteinfeger und Zuordnung zum Kehrbezirk.

## Felder

- Bestellte Person
- Kehrbezirk
- Beginn und Ende der Bestellung
- Qualifikationsnachweis
- Vertretungsregelung
- Widerruf der Bestellung

## Hinweise

Angelegt am 2026-08-03 zu `vvt-60-007` (Schornsteinfegerwesen).

Die VVT nannte „Zuständigkeiten" als Datenart -- gemeint ist der Kehrbezirk nach § 5 SchfHwG.

**Nicht enthalten: das Kehrbuch nach § 16 SchfHwG.** Es enthält Daten der Grundstückseigentümer, nicht der Schornsteinfeger. Die VVT zitiert § 16, führt Eigentümer aber nicht als Betroffene. Ob die Kommune das Kehrbuch führt oder einsieht, ist offen; falls ja, ist dafür ein eigener Speicher und eine eigene Betroffenengruppe erforderlich.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Die Bestellung ist ein hoheitlicher Akt und begründet die Zuständigkeit für einen ganzen Bezirk.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei B.** **Vertrags- und Rechtsverhältnis mit der Kommune.** Erfasst werden Vertragspartner, Gegenstand, Laufzeit und Entgelt -- Angaben, die die betroffene Person selbst ausgehandelt hat und die keine Rückschlüsse auf ihre persönlichen Verhältnisse erlauben. Bei juristischen Personen fehlt der Personenbezug ganz; erfasst sind dann nur die vertretungsberechtigten Personen mit dienstlichen Angaben.

**Anzuheben wäre der Speicher, sobald Zahlungsrückstände, Mahnungen oder Kündigungsgründe erfasst werden.** Diese Angaben gehören in `dstore-vollstreckungsdaten` beziehungsweise `dstore-mahnwesen`.

*Sammelvermerk der Durchsicht vom 2026-08-10.*
