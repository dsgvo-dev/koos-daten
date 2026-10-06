---
id: dstore-prozessaudit
bereich: intern
typ: datenspeicher
system: null
name: Prozessaudit
zuständige-einheit: oe-amt-1-1
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
    artikel: Art. 6 Abs. 1 lit. e, Art. 88
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  - gesetz: NBG
    artikel: § 88 Abs. 1
  - gesetz: NKomVG
    artikel: § 62 (Organisationshoheit)
  aufbewahrung:
    frist: 10 Jahre für Auditbericht und Maßnahmenplan; Befragungsnotizen bis zur Fertigstellung des Berichts
    beginn: nach Abschluss des Audits
    hinweis: 'Frist wie in vvt-1-1-008.'
letzte-aktualisierung: '2026-10-05'
tags:
- Organisation
- Prozessaudit
- Beschäftigtendaten
---

# Prozessaudit

## Definition

Unterlagen von Prozessaudits und Organisationsuntersuchungen in der Verwaltung: Befragungen der Beschäftigten, Auditbericht und Maßnahmenplan.

## Felder

- auditierte Organisationseinheit und Auditbereich
- befragte Beschäftigte (Name, Funktion)
- Befragungsnotizen und Ablaufbeschreibungen
- Auditbericht mit Stärken und Schwächen
- Maßnahmenplan mit Verantwortlichen und Terminen
- Umsetzungsstand

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-1-1-008 hatte bei ihrer Anlage am 06.10.2026 keinen passenden internen Speicher (OFFEN).

**Schutzstufe C.** Aussagen über die Arbeitsweise von Organisationseinheiten; keine Beurteilung einzelner Beschäftigter (diese läge auf Stufe D).

**BSI-Vektoren.** Vertraulichkeit normal, Integrität normal, Verfügbarkeit normal — keine besonderen Anforderungen.

**Abgrenzung:**
- `dstore-sitzungsprotokoll`: Protokolle von Gremiensitzungen, extern.
- `dstore-personalakte`: Beurteilungen einzelner Beschäftigter.
