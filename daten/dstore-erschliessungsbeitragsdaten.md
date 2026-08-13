---
id: dstore-erschliessungsbeitragsdaten
typ: datenspeicher
system: null
name: Erschließungsbeitragsdaten
datenkategorie: Bauen & Beiträge
zuständige-einheit: oe-amt-22
bpmn:
  typ: datenspeicher
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
  - gesetz: BauGB
  - gesetz: NKAG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Erschließung
- Beitrag
---


# Erschließungsbeitragsdaten

## Definition

Daten zur Erhebung von Erschließungsbeiträgen.

## Felder

- Grundstück
- Maßnahme
- Beitragspflichtige Person
- Verteilungsmaßstab
- Bescheid
- Fälligkeit

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-10

**B → C.** Der Erschließungsbeitrag nach §§ 127 ff. BauGB erreicht regelmäßig fünfstellige Beträge und trifft Eigentümerinnen und Eigentümer unabhängig von ihrer Leistungsfähigkeit. **Das Feld „Fälligkeit" wird deshalb in der Praxis zum Feld für Stundung, Ratenzahlung und Verrentung nach § 135 Abs. 2 bis 4 BauGB** -- und diese Angaben offenbaren wirtschaftliche Verhältnisse.

Stufe D wäre erreicht, sobald Niederschlagung oder Vollstreckung vermerkt wird.
