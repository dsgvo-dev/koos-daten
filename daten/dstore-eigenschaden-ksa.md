---
id: dstore-eigenschaden-ksa
bereich: intern
typ: datenspeicher
system: null
name: Eigenschaden und KSA-Meldung
zuständige-einheit: oe-amt-10
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
    artikel: Art. 6 Abs. 1 lit. b und lit. e
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  - gesetz: NBG
    artikel: § 90
  - gesetz: BGB
    artikel: § 280, § 619a, § 199
  - gesetz: KSA-Satzung
    artikel: Haftpflicht, Verrechnungsgrundsätze
  aufbewahrung:
    frist: 10 Jahre; bei Personenschäden 30 Jahre
    beginn: nach Abschluss des Vorgangs
    hinweis: 'Verjährungsfristen nach § 199 Abs. 3 Nr. 1 und Abs. 2 BGB, wie im Prozess proc-eigenschaden-ksa-melden beschrieben.'
letzte-aktualisierung: '2026-10-05'
tags:
- Personal
- Schaden
- KSA
- Haftung
---

# Eigenschaden und KSA-Meldung

## Definition

Schäden, die Beschäftigte der Kommune in Ausübung ihres Dienstes verursachen (Dienstfahrzeug, Dienstgerät, städtisches Eigentum), deren Meldung an den Kommunalen Schadenausgleich (KSA) Hannover, dessen Regulierung und die Prüfung eines Regresses bei grober Fahrlässigkeit.

## Felder

- schadenverursachende beschäftigte Person (Name, Dienststelle)
- Stellungnahme der beschäftigten Person
- Hergang, Ort, Zeit, Schadenshöhe, Fotos
- Fahrzeug oder Gerät (Kennzeichen, Gerätenummer, Versicherungsdaten)
- Zeuginnen und Zeugen
- Schadensmeldung an den KSA
- Regulierungsentscheidung des KSA
- Prüfung des Verschuldensgrads
- Regressbescheid und Zahlungseingang

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). Die VVT 10-030 und der Prozess nutzten bis dahin `dstore-kfz-daten` (Kfz-Zulassung), `dstore-sicherheitsmangelmeldung` (öffentlicher Raum) und `dstore-zeugenangaben-schadensfall` (Schäden an öffentlichen Straßen); keiner beschreibt Haftung und Verschulden von Beschäftigten.

**Fremdschäden nicht hier.** Ist ein Dritter geschädigt, läuft dies parallel über vvt-10-010 (Schadensmeldungen).

**Schutzstufe D.** Der Speicher enthält die Bewertung des Verschuldens einer beschäftigten Person mit möglicher Regressfolge; vergleichbar einer dienstlichen Beurteilung (Stufe D).

**BSI-Vektoren.** Vertraulichkeit hoch. Integrität normal. Verfügbarkeit normal.

**Abgrenzung:**
- `dstore-zeugenangaben-schadensfall`: Zeugen bei Schäden an öffentlichen Straßen (86-001), extern.
- `dstore-kfz-daten`: Fahrzeugzulassung, extern.
- `dstore-disziplinarvorgang`: disziplinarische Folgen; der Regress ist zivil- bzw. beamtenrechtliche Haftung, keine Disziplinarmaßnahme.
