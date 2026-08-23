---
id: dstore-meldedaten
typ: datenspeicher
system: null
name: Meldedaten
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: BMG
  - gesetz: NDSG
  aufbewahrung:
    frist: 50 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Meldedaten
- Melderegister
- Wohnsitz
konvertiert-aus: daten1/dtype-meldedaten.md
---


## Beschreibung

Daten aus dem Melderegister: Hauptwohnung, Nebenwohnung, Zuzug, Wegzug.

## Felder

- Hauptwohnung
- Nebenwohnung
- Zuzugsdatum
- Wegzugsdatum
- Meldebehörde

## Rechtsgrundlage

BMG, NDSG

## Löschfrist

50 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Das Melderegister ist Grundlage für Ausweise, Wahlen, Steuern und nahezu jede Auskunft an andere Behörden. Zusätzlich **Verfügbarkeit hoch**: Ohne Registerzugriff kann das Bürgeramt keine Leistung erbringen.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Das Melderegister ist Grundlage für Ausweise, Wahlen, Steuern und nahezu jede Auskunft an andere Behörden. Zusätzlich **Verfügbarkeit hoch**: Ohne Registerzugriff kann das Bürgeramt keine Leistung erbringen.

## Schutzstufe geprüft 2026-08-10

**D → C.** Hauptwohnung, Nebenwohnung, Zuzug, Wegzug. **Das Melderecht selbst behandelt diese Angaben nicht als besonders schutzbedürftig:** § 44 BMG erlaubt die einfache Melderegisterauskunft an jedermann ohne Darlegung eines Interesses.

Der gefährliche Fall ist nicht die Regel, sondern die Ausnahme -- und für ihn gibt es einen eigenen Speicher: `dstore-auskunftssperre-melderegister` steht auf Stufe E, weil die Sperre nach § 51 BMG eine Gefahr für Leben, Gesundheit oder Freiheit voraussetzt. **Vor jeder Auskunft ist zu prüfen, ob eine Sperre oder ein bedingter Sperrvermerk nach § 52 BMG vorliegt.** Diese Prüfung ist die eigentliche Schutzmaßnahme; sie wird durch eine pauschal hohe Einstufung nicht ersetzt.
