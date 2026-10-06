---
id: dstore-rechtsberatung-intern
bereich: intern
typ: datenspeicher
system: null
name: Rechtsberatung intern
zuständige-einheit: oe-amt-30
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
    artikel: Art. 6 Abs. 1 lit. e
  - gesetz: NDSG
    artikel: § 3, § 12 Abs. 1
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Abschluss des Vorgangs
    hinweis: 'Frist wie in vvt-30-003 (kommunale Aktenordnung).'
letzte-aktualisierung: '2026-10-05'
tags:
- Recht
- Beratung
---

# Rechtsberatung intern

## Definition

Anfragen der Ämter an das Rechtsamt und deren Beantwortung.

## Felder

- anfragende Person und Amt (dienstliche Kontaktdaten)
- Sachverhalt und Fragestellung
- beigezogene Unterlagen
- rechtliche Prüfung
- Stellungnahme oder Empfehlung
- Wiedervorlage und Abschluss

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-30-003 nutzte bis dahin `dstore-beratungsdokumentation` (Bürgerberatung), `dstore-kontaktdaten` und `dstore-personenstammdaten`, alle extern.

**Schutzstufe C.** Sachverhalte können personenbezogene Angaben Dritter enthalten, etwa aus Personal- oder Vertragsangelegenheiten.

**BSI-Vektoren.** Vertraulichkeit normal, Integrität normal, Verfügbarkeit normal — keine besonderen Anforderungen.

**Abgrenzung:**
- `dstore-beratungsdokumentation`: Beratung von Bürgerinnen und Bürgern, extern.
- `dstore-vergabeunterlagen`: Unterlagen des Vergabeverfahrens; die Beratung sieht sie ein, führt sie nicht.
