---
id: dstore-bem-verfahrensdaten
typ: datenspeicher
system: null
name: Betriebliches Eingliederungsmanagement (BEM) — Verfahrensdaten
zuständige-einheit: oe-amt-11
bpmn:
  typ: nachricht
klassifizierung:
  # Datenschutz — Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit — Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
rechtsgrundlagen:
  - gesetz: SGB IX
    artikel: § 167 Abs. 2
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. a und lit. b
  - gesetz: DSGVO
    artikel: Art. 88
  - gesetz: NDSG
    artikel: § 3
  - gesetz: NDSG
    artikel: § 12
  - gesetz: NDSG
    artikel: § 17
  - gesetz: NBG
    artikel: §§ 88, 45 Abs. 2
  - gesetz: NPersVG
    artikel: § 81-Vereinbarung
aufbewahrung:
  frist: 3 Jahre
  beginn: nach Beendigung des Dienst- oder Arbeitsverhältnisses
  hinweis: 'Deckungsgleich mit VVT vvt-11-009. BEM-Verfahrensdaten sind getrennt von der übrigen Personalakte zu führen (§ 45 Abs. 2 NBG: versiegelter Umschlag für Gesundheitsdaten).'
letzte-aktualisierung: '2026-10-02'
tags:
  - BEM
  - Betriebliches Eingliederungsmanagement
  - Gesundheitsdaten
  - Beschäftigtendatenschutz
  - Einwilligung
---

# Betriebliches Eingliederungsmanagement (BEM) — Verfahrensdaten

## Definition

Verfahrensbezogene Daten des betrieblichen Eingliederungsmanagements nach § 167 Abs. 2 SGB IX, die ausschließlich innerhalb der abgetrennten BEM-Stelle verarbeitet werden. Umfasst die Dokumentation des BEM-Angebots, der Einwilligung der beschäftigten Person, der BEM-Gespräche und der vereinbarten Maßnahmen.

**Abgrenzung:** `dstore-arbeitsunfaehigkeit-krankheit` enthält die AU-Zeiten für die Fristberechnung (Sechs-Wochen-Frist). Die eigentlichen BEM-Verfahrensdaten werden getrennt davon in diesem Speicher geführt — entsprechend der Trennung von Personalakte und BEM-Akte.

## Felder

- BEM-Angebot (Datum, Unterrichtungsschreiben)
- Einwilligung / Ablehnung (Ankreuzverfahren nach BVerwG 6 P 8.09)
- BEM-Gesprächsdokumentation (Datum, Teilnehmer, Inhalte)
- Maßnahmenplan (vereinbarte Maßnahmen, Wiedereingliederung, Arbeitsplatzanpassung)
- Zugriffsprotokoll (wer hat wann auf die BEM-Akte zugegriffen)

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: nachricht

## Rechtsgrundlagen

- § 167 Abs. 2 SGB IX (BEM-Verfahren)
- Art. 9 Abs. 2 lit. a DSGVO (Einwilligung in Gesundheitsdatenverarbeitung)
- Art. 9 Abs. 2 lit. b DSGVO (Fristberechnung aus Krankheitstagen)
- Art. 88 DSGVO (Beschäftigtendatenschutz)
- § 3 NDSG, § 12 NDSG, § 17 NDSG
- §§ 88, 45 Abs. 2 NBG (Personalaktenführung, getrennte Aufbewahrung von Gesundheitsdaten)
- § 81-Vereinbarung NPersVG (BEM in der nds. Landesverwaltung)

## Aufbewahrung

- **Frist:** 3 Jahre
- **Beginn:** nach Beendigung des Dienst- oder Arbeitsverhältnisses
- **Hinweis:** Die BEM-Akte ist von der Personalakte getrennt zu führen. Gesundheitsdaten sind in einem verschlossenen Umschlag und versiegelt zur Personalakte zu nehmen (§ 45 Abs. 2 NBG). Die Frist ist deckungsgleich mit VVT vvt-11-009.

## Verwendung in Prozessen

- Betriebliches Eingliederungsmanagement durchführen (proc-bem-durchfuehren)

## BSI-Vektoren — Begründung

**Vertraulichkeit: hoch.** Art. 9 DSGVO-Daten (Gesundheitsdaten) mit strenger Zweckbindung. Die LfD Niedersachsen betont, dass nur beauftragte Personen Zugang haben dürfen — nicht Fachvorgesetzte. Daten aus BEM-Gesprächen dürfen nicht in die allgemeine Personalakte oder an Dritte gelangen. Ein unbefugter Zugriff gefährdet das Vertrauensverhältnis, das für das BEM-Verfahren konstitutiv ist.

**Integrität: normal.** Die BEM-Akte dokumentiert Gesprächsinhalte und Vereinbarungen — sie ist kein Register, auf dessen Richtigkeit sich Dritte verlassen. Anders als bei Melderegistern oder Grundbucheinträgen wirkt sich eine versehentlich falsche Eintragung nur auf das konkrete BEM-Verfahren aus. Die Korrekturmöglichkeit über § 16 DSGVO ist ausreichend.

**Verfügbarkeit: normal.** Das BEM-Verfahren läuft über Wochen und Monate. Ein kurzfristiger Ausfall des Zugriffs verzögert das Verfahren, verhindert es aber nicht. Die Verfügbarkeit ist nicht zeitkritisch — anders als bei Systemen der Gefahrenabwehr oder Notfallversorgung.

## Hinweise

Dieser Datenspeicher wurde am 2026-10-02 neu angelegt, um die BEM-Verfahrensdaten vom allgemeinen Krankenstands-Datenspeicher (`dstore-arbeitsunfaehigkeit-krankheit`) zu trennen. Hintergrund: Die BEM-Stelle arbeitet organisatorisch abgetrennt und verarbeitet Daten des BEM-Verfahrens (Angebot, Annahme, Vereinbarungen), die nicht in den allgemeinen AU-Datenbestand gehören.

Quelle für die fachliche Einordnung: LfD Niedersachsen, „Hinweise zum Betrieblichen Eingliederungsmanagement (BEM)", Stand 27.10.2020.