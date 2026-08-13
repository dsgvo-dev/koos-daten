---
id: dstore-maulkorb-leinenanordnung
typ: datenspeicher
system: null
name: Maulkorb- und Leinenanordnung
datenkategorie: Ordnung & Tiere
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
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
  - gesetz: NHundG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-12'
tags:
- Hund
- Maulkorb
- Leine
---


# Maulkorb- und Leinenanordnung

## Definition

Ordnungsrechtliche Anordnungen zu Leinen- oder Maulkorbpflichten.

## Felder

- Betroffene Person
- Hund
- Anlass
- Anordnungsumfang
- Zeitraum
- Aktenzeichen

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit hoch.** Der Bestand dient der Gefahrenabwehr. Ist er verfälscht oder im entscheidenden Moment nicht abrufbar, kann die Kommune ihre Schutzaufgabe nicht erfüllen -- mit möglichen Folgen für Leib und Leben.

Die Anordnung dient dem Schutz Dritter vor einem als gefährlich eingestuften Hund. Sie muss im Kontrollfall abrufbar und unverfälscht sein.

## Schutzstufe geprüft 2026-08-12

**Bleibt bei C.** **§ 9 NHundG** knüpft Leinen- und Maulkorbpflicht an die Feststellung der Gefährlichkeit nach § 7 NHundG; daneben kann die Gemeinde solche Pflichten im Einzelfall anordnen.

Das Feld „Anlass" nennt den Vorfall, das Feld „Betroffene Person" die Halterin. Eine belastende Ordnungsverfügung gegen eine namentlich benannte Person beeinträchtigt deren gesellschaftliche Stellung.

**Lücke im Verzeichnis.** Der Speicher steht auf `verwendungen: 0`, gehört sachlich aber zu `vvt-71-002` (Tierschutz, gefährliche Hunde). Die Kommune führt diese Daten; das Verzeichnis weist sie nicht aus. Als eigener Auftrag vorgemerkt, siehe den Vorschlag zu Los 1, Abschnitt 4a.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
