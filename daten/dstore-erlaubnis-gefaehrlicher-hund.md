---
id: dstore-erlaubnis-gefaehrlicher-hund
typ: datenspeicher
system: null
name: Erlaubnis gefährlicher Hund
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
- Gefährlich
- Erlaubnis
---



# Erlaubnis gefährlicher Hund

## Definition

Erlaubnisdaten für die Haltung eines gefährlichen Hundes.

## Felder

- Hundehalter/in
- Hund
- Erlaubnisstatus
- Sachkunde
- Haftpflicht
- Haltungsort

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** Der Bestand wird in einer Gefahrenlage gebraucht, in der es auf Minuten ankommt. Ein Ausfall bedeutet, dass die Kommune die Lage nicht einschätzen kann.

Die Erlaubnis samt Auflagen muss im Kontrollfall vorliegen.

## Schutzstufe geprüft 2026-08-12

**Bleibt bei C.** Nach **§ 7 NHundG** stellt die Behörde die Gefährlichkeit eines Hundes im Einzelfall durch Verwaltungsakt fest; **§ 8 NHundG** stellt das Halten eines solchen Hundes unter Erlaubnisvorbehalt.

Der Eintrag belegt damit, dass gegen die Halterin oder den Halter ein ordnungsrechtlicher Vorgang geführt wurde — häufig nach einem Beißvorfall. Das beeinträchtigt die gesellschaftliche Stellung in der Nachbarschaft.

**Abgrenzung.** Die Speicher zur gewöhnlichen Hundehaltung sind am 2026-08-12 auf B herabgestuft worden. Der Unterschied ist nicht der Hund, sondern der Verwaltungsakt.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
