---
id: dstore-gefaehrdungsbeurteilung
bereich: intern
typ: datenspeicher
system: null
name: Gefährdungsbeurteilung
zuständige-einheit: oe-amt-11
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
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  - gesetz: ArbSchG
    artikel: § 5, § 6
  - gesetz: ArbStättV
    artikel: § 3
  - gesetz: DGUV Vorschrift 1
    artikel: § 3
  aufbewahrung:
    frist: bis zur nächsten Aktualisierung, mindestens 3 Jahre
    beginn: nach Außerbetriebnahme des Arbeitsplatzes
    hinweis: 'Frist wie in vvt-11-013.'
letzte-aktualisierung: '2026-10-05'
tags:
- Personal
- Arbeitsschutz
- Gefährdungsbeurteilung
---

# Gefährdungsbeurteilung

## Definition

Gefährdungsbeurteilungen nach § 5 ArbSchG für Arbeitsplätze und Tätigkeiten der Kommune mit Maßnahmen und Wirksamkeitskontrolle, dokumentiert nach § 6 ArbSchG.

## Felder

- Arbeitsplatz oder Tätigkeit
- dort tätige Beschäftigte (Namen)
- ermittelte Gefährdungen (physisch, psychisch, biologisch, chemisch)
- Beurteilungsergebnis
- Maßnahmen mit Termin und verantwortlicher Person
- Wirksamkeitskontrolle und Fortschreibung
- Beteiligung von Fachkraft für Arbeitssicherheit, Betriebsärztin oder Betriebsarzt und Personalrat

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). Die VVT 11-013 nutzte bis dahin `dstore-ausbildungsnachweis-station` (Referendarstation) — eine Fehlzuordnung, die am 05.10.2026 beseitigt wurde.

**Keine Gesundheitsbefunde.** Arbeitsmedizinische Befunde stehen nur in der Akte der Betriebsärztin oder des Betriebsarztes. Dass eine Vorsorge stattfand, steht in `dstore-vorsorgekartei`.

**Schutzstufe C.** Arbeitsplatzbezogene Beurteilung mit Namensbezug, ohne Gesundheitsdaten.

**BSI-Vektoren.** Alle normal.

**Abgrenzung:**
- `dstore-vorsorgekartei`: personenbezogene Vorsorge, eigene Frist.
- `dstore-ausbildungsnachweis-station`: Referendarstation, extern.
