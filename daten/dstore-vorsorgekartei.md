---
id: dstore-vorsorgekartei
bereich: intern
typ: datenspeicher
system: null
name: Vorsorgekartei (arbeitsmedizinische Vorsorge)
zuständige-einheit: oe-amt-11
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
    artikel: Art. 6 Abs. 1 lit. c, Art. 9 Abs. 2 lit. b
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  - gesetz: ArbMedVV
    artikel: § 3 Abs. 4
  aufbewahrung:
    frist: bis zur Beendigung des Beschäftigungsverhältnisses
    beginn: Beendigung des Beschäftigungsverhältnisses
    hinweis: '§ 3 Abs. 4 ArbMedVV: aufzubewahren bis zur Beendigung des Beschäftigungsverhältnisses und anschließend zu löschen; bei Beendigung erhält die Person eine Kopie der sie betreffenden Angaben.'
letzte-aktualisierung: '2026-10-05'
tags:
- Personal
- Arbeitsschutz
- Arbeitsmedizinische Vorsorge
---

# Vorsorgekartei (arbeitsmedizinische Vorsorge)

## Definition

Vorsorgekartei des Arbeitgebers nach § 3 Abs. 4 ArbMedVV mit Angaben, dass, wann und aus welchen Anlässen arbeitsmedizinische Vorsorge stattgefunden hat.

## Felder

- Name und Personalnummer
- Anlass der Vorsorge (Pflicht-, Angebots- oder Wunschvorsorge; Tätigkeit)
- Datum der Vorsorge
- Datum der nächsten Vorsorge
- Vorsorgebescheinigung (nur Teilnahme, kein Befund)

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). Die VVT 11-013 nutzte für die arbeitsmedizinische Vorsorge bis dahin `dstore-arbeitsunfaehigkeit-krankheit` als Behelfspeicher; Vorsorge ist keine Arbeitsunfähigkeit (Entscheidung Martin 05.10.2026, Option A).

**Keine Befunde.** Befunde bleiben bei der Betriebsärztin oder dem Betriebsarzt; der Arbeitgeber erhält nur die Vorsorgebescheinigung.

**Schutzstufe D.** Die Kartei hält nur fest, dass, wann und aus welchem Anlass eine Vorsorge stattfand, nicht deren Ergebnis. Schon Anlass und Teilnahme können aber auf den Gesundheitszustand schließen lassen (etwa eine Wunschvorsorge); die VVT 11-013 stützt die Vorsorge deshalb auf Art. 9 Abs. 2 lit. b DSGVO. Am 05.10.2026 von C auf D angehoben, weil die Prüfung für Art.-9-Verarbeitungen einen Speicher der Stufe D verlangt.

**BSI-Vektoren.** Vertraulichkeit hoch (folgt der Schutzstufe). Integrität und Verfügbarkeit normal.

**Abgrenzung:**
- `dstore-gefaehrdungsbeurteilung`: arbeitsplatzbezogen; die Vorsorgeanlässe folgen aus ihr.
- `dstore-arbeitsunfaehigkeit-beschaeftigte`: Arbeitsunfähigkeit, nicht Vorsorge.
