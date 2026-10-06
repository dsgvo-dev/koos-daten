---
id: dstore-beschaffungsvorgang
bereich: intern
typ: datenspeicher
system: null
name: Beschaffungsvorgang
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
    artikel: Art. 6 Abs. 1 lit. b und lit. e
  - gesetz: NDSG
    artikel: § 3
  - gesetz: NKomVG
    artikel: § 110 (Haushaltsgrundsätze)
  - gesetz: KomHKVO
    artikel: Belege und Aufbewahrung
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Ablauf des Haushaltsjahres
    hinweis: 'Frist wie in vvt-10-025 (steuerliche Aufbewahrungsfrist).'
letzte-aktualisierung: '2026-10-05'
tags:
- Beschaffung
- Haushalt
---

# Beschaffungsvorgang

## Definition

Interne Bestell- und Beschaffungsvorgänge der Kommune von der Bestellanforderung bis zum Auftrag.

## Felder

- anfordernde Person und Organisationseinheit
- Bestellposten
- Kostenstelle und Haushaltsstelle
- Lieferant und Ansprechperson
- Auftrag oder Vertragsbezug
- Freigabevermerk

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). Die Bestellanforderung (vvt-10-025), die Einführung von IT-Verfahren (vvt-15-004), die Rechnungsbearbeitung (vvt-20-004) und die Prozesse `proc-bestellanforderung`, `proc-it-einfuehrung`, `proc-ausschreibungen-veroeffentlichen` nutzten bis dahin `dstore-vergabe-auftragsbezug` und `dstore-rechnungsdaten`, beide extern.

**Schutzstufe B.** Namen und dienstliche Kontaktdaten von Beschäftigten und Ansprechpersonen der Lieferanten; keine sensiblen Angaben.

**BSI-Vektoren.** Vertraulichkeit normal, Integrität normal, Verfügbarkeit normal — ein Fehler wirkt sich auf den einzelnen Vorgang aus.

**Abgrenzung:**
- `dstore-vergabe-auftragsbezug`: Vergabeverfahren gegenüber Bietenden, extern.
- `dstore-debitoren-kreditorendaten`: Stammdaten der Lieferanten als Zahlungsempfänger.
- `dstore-elektronische-rechnungsstellung`: eingehende Rechnungen.
