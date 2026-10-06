---
id: dstore-ideenmanagement
bereich: intern
typ: datenspeicher
system: null
name: Ideenmanagement
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
    artikel: § 12 Abs. 1
  aufbewahrung:
    frist: Anonymisierung nach 3 Jahren, Löschung nach 5 Jahren
    beginn: nach Abschluss des Vorgangs oder der Umsetzung
    hinweis: 'Frist wie in vvt-10-019.'
letzte-aktualisierung: '2026-10-05'
tags:
- Personal
- Ideenmanagement
---

# Ideenmanagement

## Definition

Verbesserungsvorschläge der Beschäftigten, ihre Bewertung, Prämierung und Umsetzung.

## Felder

- einreichende Person und Organisationseinheit
- Vorschlag
- Bewertung und Gutachten
- Entscheidung und Prämie
- Umsetzung

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). `proc-ideen-und-verbesserungsvorschlaege-bearbeiten` nutzte bis dahin `dstore-beschwerde-anregungsdaten` (Bürgerbeschwerden), `dstore-kontaktdaten` und `dstore-personenstammdaten`, alle extern.

**Schutzstufe B.** Dienstliche Angaben und Prämienhöhe.

**BSI-Vektoren.** Vertraulichkeit normal, Integrität normal, Verfügbarkeit normal — keine besonderen Anforderungen.

**Abgrenzung:**
- `dstore-beschwerde-anregungsdaten`: Eingaben von Bürgerinnen und Bürgern, extern.
