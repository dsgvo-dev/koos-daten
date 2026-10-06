---
id: dstore-bem-verfahrensdaten
bereich: intern
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
    artikel: § 88 Abs. 3, § 45 Abs. 2 Satz 2, § 94 Abs. 2
  - gesetz: NPersVG
    artikel: § 60 Abs. 1 und Abs. 2 Nr. 2
  - gesetz: NPersVG
    artikel: § 78 (Dienstvereinbarung BEM, reg-dv-bem)
aufbewahrung:
  frist: 3 Jahre
  beginn: 'BEM-Akte: nach Abschluss des BEM-Verfahrens; Teilakte BEM-Nachweise: nach Beendigung des Dienst- oder Arbeitsverhältnisses'
  hinweis: 'Deckungsgleich mit VVT vvt-11-009. Aufteilung nach dem Muster JLU Gießen: Teilakte BEM-Nachweise (Angebot, Unterrichtungsschreiben, Antwort, Abschlussvermerk) und BEM-Akte (Gesprächsdokumentation, Maßnahmenplan, Ergebnis), beide als Teilakten zur Personalakte (§ 88 Abs. 3 NBG). Unterlagen mit Angaben zur Art der Erkrankung verschlossen (§ 45 Abs. 2 Satz 2 NBG) und unverzüglich vernichten, sobald nicht mehr erforderlich.'
letzte-aktualisierung: '2026-10-05'
tags:
  - BEM
  - Betriebliches Eingliederungsmanagement
  - Gesundheitsdaten
  - Beschäftigtendatenschutz
  - Einwilligung
---

# Betriebliches Eingliederungsmanagement (BEM) — Verfahrensdaten

## Definition

Verfahrensbezogene Daten des betrieblichen Eingliederungsmanagements nach § 167 Abs. 2 SGB IX. Umfasst die Dokumentation des BEM-Angebots, der Einwilligung der beschäftigten Person, der BEM-Gespräche und der vereinbarten Maßnahmen.

Die Daten werden in zwei Teilakten zur Personalakte geführt (§ 88 Abs. 3 NBG; Muster JLU Gießen):
- **Teilakte BEM-Nachweise** (Personalstelle): Angebot, Unterrichtungsschreiben, Antwort, Abschlussvermerk.
- **BEM-Akte** (nur BEM-Beauftragte): Gesprächsdokumentation, Maßnahmenplan, Ergebnis. In der Personalakte steht nur ein Hinweis auf ihre Existenz.

**Abgrenzung:** `dstore-arbeitsunfaehigkeit-beschaeftigte` enthält die AU-Zeiten für die Fristberechnung (Sechs-Wochen-Frist). Die eigentlichen BEM-Verfahrensdaten werden getrennt davon in diesem Speicher geführt — entsprechend der Trennung von Personalakte und BEM-Akte.

## Felder

Teilakte BEM-Nachweise:
- BEM-Angebot (Datum, Unterrichtungsschreiben)
- Antwort im Ankreuzverfahren (nach BVerwG 6 P 8.09 und LfD Niedersachsen): Zustimmung mit oder ohne Beteiligung von Personalrat/Schwerbehindertenvertretung, Ablehnung, Einwilligung in die Beteiligung weiterer Personen, Wunsch nach späterem Angebot
- Widerruf (Datum)
- Wiedervorlage für ein erneutes Angebot
- Abschlussvermerk (Datum, Beendigungsgrund; keine Gesundheitsdaten)

BEM-Akte:
- Einwilligungen in die Beteiligung Dritter (Personalrat, Schwerbehindertenvertretung, Betriebsarzt, Vertrauensperson, Fachvorgesetzte, externe Stellen)
- BEM-Gesprächsdokumentation (Datum, Teilnehmer, Inhalte)
- Maßnahmenplan (vereinbarte Maßnahmen, Wiedereingliederung, Arbeitsplatzanpassung) und Ergebnis
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
- § 88 Abs. 3 NBG (Teilakten), § 45 Abs. 2 Satz 2 NBG (verschlossene Aufbewahrung von Gesundheitsunterlagen), § 94 Abs. 2 NBG (frühere Löschung von Teilakten)
- § 60 Abs. 1 und Abs. 2 Nr. 2 NPersVG (Unterrichtung des Personalrats: Namen und Unterrichtungsschreiben)
- Dienstvereinbarung BEM nach § 78 NPersVG (reg-dv-bem). Die § 81-Vereinbarung gilt nur für die Landesverwaltung und ist für Kommunen keine Rechtsgrundlage.

## Aufbewahrung

- **BEM-Akte:** 3 Jahre nach Abschluss des BEM-Verfahrens
- **Teilakte BEM-Nachweise:** 3 Jahre nach Beendigung des Dienst- oder Arbeitsverhältnisses
- **Unterlagen mit Angaben zur Art der Erkrankung:** verschlossen und versiegelt zur Akte (§ 45 Abs. 2 Satz 2 NBG); unverzüglich vernichten, sobald nicht mehr erforderlich
- **Hinweis:** Die Fristen sind deckungsgleich mit VVT vvt-11-009.

## Verwendung in Prozessen

- Betriebliches Eingliederungsmanagement durchführen (proc-bem-durchfuehren)

## BSI-Vektoren — Begründung

**Vertraulichkeit: hoch.** Art. 9 DSGVO-Daten (Gesundheitsdaten) mit strenger Zweckbindung. Die LfD Niedersachsen betont, dass nur beauftragte Personen Zugang haben dürfen — nicht Fachvorgesetzte. Daten aus BEM-Gesprächen dürfen nicht in die allgemeine Personalakte oder an Dritte gelangen. Ein unbefugter Zugriff gefährdet das Vertrauensverhältnis, das für das BEM-Verfahren konstitutiv ist.

**Integrität: normal.** Die BEM-Akte dokumentiert Gesprächsinhalte und Vereinbarungen — sie ist kein Register, auf dessen Richtigkeit sich Dritte verlassen. Anders als bei Melderegistern oder Grundbucheinträgen wirkt sich eine versehentlich falsche Eintragung nur auf das konkrete BEM-Verfahren aus. Die Korrekturmöglichkeit über § 16 DSGVO ist ausreichend.

**Verfügbarkeit: normal.** Das BEM-Verfahren läuft über Wochen und Monate. Ein kurzfristiger Ausfall des Zugriffs verzögert das Verfahren, verhindert es aber nicht. Die Verfügbarkeit ist nicht zeitkritisch — anders als bei Systemen der Gefahrenabwehr oder Notfallversorgung.

## Hinweise

Dieser Datenspeicher wurde am 2026-10-02 neu angelegt, um die BEM-Verfahrensdaten vom allgemeinen Krankenstands-Datenspeicher (`dstore-arbeitsunfaehigkeit-krankheit`) zu trennen. Hintergrund: Die BEM-Stelle arbeitet organisatorisch abgetrennt und verarbeitet Daten des BEM-Verfahrens (Angebot, Annahme, Vereinbarungen), die nicht in den allgemeinen AU-Datenbestand gehören. Am 2026-10-05 auf zwei Teilakten (Muster JLU Gießen) umgestellt; die Rechtsgrundlage § 81-Vereinbarung durch § 60 und § 78 NPersVG ersetzt.

Quelle für die fachliche Einordnung: LfD Niedersachsen, „Hinweise zum Betrieblichen Eingliederungsmanagement (BEM)", Stand 27.10.2020.