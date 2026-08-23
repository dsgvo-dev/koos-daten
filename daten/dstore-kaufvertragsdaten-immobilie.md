---
id: dstore-kaufvertragsdaten-immobilie
typ: datenspeicher
system: null
name: Kaufvertragsdaten Immobilie
zuständige-einheit: oe-amt-23
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: BGB
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-04'
tags:
- Kaufvertrag
- Immobilie
---


# Kaufvertragsdaten Immobilie

## Definition

Daten zu kommunalen oder privat vorgelegten Kaufverträgen über Immobilien.

## Felder

- Vertragsparteien
- Objekt
- Kaufpreis
- Beurkundungsdatum
- Notariat
- Fälligkeitsbedingungen

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## Schutzstufe geprüft 2026-08-04

Durchsicht des Katalogs gegen das Schutzstufenkonzept des LfD Niedersachsen,
Maximalprinzip.

**Von B auf C.** Der Speicher führt Kaufpreis, Vertragsparteien und Fälligkeitsbedingungen. Das Schutzstufenkonzept ordnet der Stufe C Daten zu, deren Missbrauch die **wirtschaftlichen Verhältnisse** beeinträchtigen kann -- der Kaufpreis einer Immobilie gehört dazu.

Der Speicher wird in sechs Verarbeitungstätigkeiten geführt, darunter die Vorkaufsrechtsprüfung (`vvt-23-006`, `vvt-63-004`) und die sanierungsrechtliche Prüfung nach § 138 BauGB (`vvt-64-002`).

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*
