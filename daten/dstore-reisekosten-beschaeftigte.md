---
id: dstore-reisekosten-beschaeftigte
bereich: intern
typ: datenspeicher
system: null
name: Reisekosten der Beschäftigten
zuständige-einheit: oe-amt-10
personenbezug: ja
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. b und lit. c
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  - gesetz: NBG
    artikel: § 84, § 94 Abs. 2
  - gesetz: NRKVO
    artikel: Niedersächsische Reisekostenverordnung
  - gesetz: TVöD
    artikel: tarifliche Verweisung auf das Reisekostenrecht der Beamtinnen und Beamten
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Ablauf des Jahres, in dem die Bearbeitung des einzelnen Vorgangs abgeschlossen wurde
    hinweis: '§ 94 Abs. 2 Satz 1 NBG für Reise- und Umzugskostenvergütungen; gilt nach § 12 Abs. 1 NDSG auch für Tarifbeschäftigte.'
letzte-aktualisierung: '2026-10-05'
tags:
- Personal
- Dienstreise
- Reisekosten
---

# Reisekosten der Beschäftigten

## Definition

Dienstreisen der Beschäftigten von Antrag und Genehmigung bis zur Abrechnung der Reisekostenvergütung.

## Felder

- Name, Vorname, Personalnummer
- Reiseziel, -dauer, -zweck
- Genehmigungsvermerk
- Fahrt-, Übernachtungs- und Nebenkosten mit Belegen
- Tagegeld
- Erstattungsbetrag
- Bankverbindung (Verweis auf Personalstammdaten)

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-11-010 und `proc-dienstreise` nutzten bis dahin `dstore-aufwandsentschaedigung-ehrenamt`; die VVT nannte ihn selbst Behelfspeicher.

**Schutzstufe C.** Reiseziele und -zeiten lassen Aufenthalte der Beschäftigten erkennen.

**BSI-Vektoren.** Vertraulichkeit normal, Integrität normal, Verfügbarkeit normal — keine besonderen Anforderungen.

**Abgrenzung:**
- `dstore-aufwandsentschaedigung-ehrenamt`: Entschädigungen Ehrenamtlicher, extern.
