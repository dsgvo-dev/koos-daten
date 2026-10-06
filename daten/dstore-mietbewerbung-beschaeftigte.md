---
id: dstore-mietbewerbung-beschaeftigte
bereich: intern
typ: datenspeicher
system: null
name: Mietbewerbung Beschäftigte
zuständige-einheit: oe-amt-23
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
    artikel: Art. 6 Abs. 1 lit. b
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  - gesetz: AGG
    artikel: § 19, § 21 Abs. 5, § 22
  aufbewahrung:
    frist: 6 Monate
    beginn: nach der Absage
    hinweis: 'Frist wie in vvt-23-004 (Zweimonatsfrist § 21 Abs. 5 AGG zuzüglich Zuschlag); bei Vertragsschluss Übergang in `dstore-mietvertrag`.'
letzte-aktualisierung: '2026-10-05'
tags:
- Wohnung
- Vermietung
- Beschäftigtendaten
---

# Mietbewerbung Beschäftigte

## Definition

Bewerbungen von Beschäftigten um eine Wohnung der Kommune und die Vergabeentscheidung. Die Kommune vermietet nur an Beschäftigte (Martin, 05.10.2026).

## Felder

- bewerbende beschäftigte Person (Name, Anschrift, Kontaktdaten)
- Haushaltsgröße und -zusammensetzung
- bisherige Wohnsituation und Wohnungswunsch
- Einkommensangaben, soweit für die Vergabe erheblich
- Wohnberechtigungsschein, soweit vorgelegt
- Vergabeentscheidung und Auswahldokumentation

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-23-004 und `proc-mietbewerbung-verwalten-und-wohnung-vergeben` nutzten bis dahin `dstore-wohnberechtigung`, `dstore-einkommensnachweise-haushalt` und `dstore-wohnungszuordnungsmerkmal`, alle extern.

**Schutzstufe D.** Einkommen und Haushaltsverhältnisse sind finanzielle Verhältnisse; Stufe wie die bisher genutzten Einkommensspeicher.

**BSI-Vektoren.** Vertraulichkeit hoch, Integrität normal, Verfügbarkeit normal — Vertraulichkeit hoch wegen der Einkommensangaben.

**Abgrenzung:**
- `dstore-mietvertrag`: abgeschlossener Mietvertrag.
- `dstore-wohnberechtigung`: Wohnberechtigungsschein-Verfahren, extern.
