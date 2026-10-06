---
id: dstore-gesundheitliche-eignung
bereich: intern
typ: datenspeicher
system: null
name: Gesundheitliche Eignung
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
    artikel: Art. 9 Abs. 2 lit. b
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  - gesetz: NBG
    artikel: § 88 Abs. 1, § 94
  - gesetz: BeamtStG
    artikel: § 9
  aufbewahrung:
    frist: 5 Jahre nach Abschluss der Personalakte; bei Bewerbenden ohne Einstellung 6 Monate nach Absage
    beginn: siehe Frist
    hinweis: 'Bei Einstellung Teil der Personalakte (§ 94 Abs. 1 NBG); bei Absage wie Bewerbungsunterlagen (§ 15 Abs. 4 AGG).'
letzte-aktualisierung: '2026-10-05'
tags:
- Personal
- Gesundheitsdaten
- Eignung
---

# Gesundheitliche Eignung

## Definition

Ergebnis ärztlicher Untersuchungen der gesundheitlichen Eignung von Bewerbenden und Auszubildenden (geeignet, nicht geeignet, geeignet mit Einschränkungen). Befunde bleiben bei der untersuchenden Ärztin oder dem untersuchenden Arzt.

## Felder

- Name der untersuchten Person
- Anlass (Einstellung, Ausbildung, Verbeamtung)
- untersuchende Stelle
- Datum
- Ergebnis der Eignung
- Einschränkungen, soweit für den Einsatz erheblich

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-11-001 (einstellungsärztliche Untersuchung) und vvt-11-006 (gesundheitliche Eignung) nutzten bis dahin `dstore-gesundheitsdaten`, extern.

**Schutzstufe D.** Auch das Ergebnis allein ist ein Gesundheitsdatum nach Art. 9 Abs. 1 DSGVO.

**BSI-Vektoren.** Vertraulichkeit hoch, Integrität normal, Verfügbarkeit normal — Vertraulichkeit hoch.

**Abgrenzung:**
- `dstore-gesundheitsdaten`: Gesundheitsdaten in Bürgerverfahren, extern.
- `dstore-arbeitsunfaehigkeit-beschaeftigte`: Arbeitsunfähigkeit, nicht Eignung.
