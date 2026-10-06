---
id: dstore-beschaeftigungsnachweis
bereich: extern
typ: datenspeicher
system: null
name: Beschäftigungsnachweis
zuständige-einheit: oe-amt-50
personenbezug: ja
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: NDSG
    artikel: § 3
  - gesetz: SGB X
    artikel: § 67 ff. (soweit Sozialdaten)
  - gesetz: SGB II
    artikel: § 60
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Abschluss des Verfahrens
    hinweis: 'Frist wie in vvt-32-005 und vvt-50-010.'
letzte-aktualisierung: '2026-10-05'
tags:
- Beschäftigung
- Nachweis
- Sozialdaten
---

# Beschäftigungsnachweis

## Definition

Angaben und Nachweise über die Beschäftigung von Bürgerinnen und Bürgern bei Dritten, soweit ein Verwaltungsverfahren sie voraussetzt (etwa Fahrerbescheinigung, Grundsicherung für Arbeitsuchende).

## Felder

- Person
- Arbeitgeber
- Art der Beschäftigung
- Beginn und Ende
- Arbeitszeit
- Beschäftigungs- oder Verdienstnachweis

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-32-005 und vvt-50-010 nutzten bis dahin `dstore-arbeitsverhaeltnis-beschaeftigung`, der seit 05.10.2026 die Beschäftigten der Kommune beschreibt (intern).

**Schutzstufe D.** Im SGB-II-Verfahren sind Beschäftigungsangaben Sozialdaten (Sozialgeheimnis, § 35 SGB I).

**BSI-Vektoren.** Vertraulichkeit hoch, Integrität normal, Verfügbarkeit normal — Vertraulichkeit hoch wegen des Sozialgeheimnisses.

**Abgrenzung:**
- `dstore-arbeitsverhaeltnis-beschaeftigung`: Beschäftigte der Kommune, intern.
- `dstore-einkommensdaten`: Einkommen in Leistungsverfahren.
