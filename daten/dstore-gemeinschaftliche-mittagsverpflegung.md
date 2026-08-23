---
id: dstore-gemeinschaftliche-mittagsverpflegung
typ: datenspeicher
system: null
name: Gemeinschaftliche Mittagsverpflegung
zuständige-einheit: oe-amt-40
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: normal
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: SGB II
  - gesetz: BKGG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Mittagessen
- Schule
- Kita
---


# Gemeinschaftliche Mittagsverpflegung

## Definition

Daten zur Teilnahme an gemeinschaftlicher Mittagsverpflegung in Schule oder Kita.

## Felder

- Einrichtung
- Teilnehmende Person
- Zeitraum
- Verpflegungsart
- Eigenanteil
- Kosten

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

**C → D.** Die Leistung wird nur gewährt, wenn die Familie hilfebedürftig ist -- § 28 SGB II, § 34 SGB XII und § 6b BKGG knüpfen sie an den Bezug von Bürgergeld, Sozialhilfe, Wohngeld oder Kinderzuschlag. **Die Datenart offenbart deshalb aus sich heraus den Leistungsbezug einer Familie**, auch wenn kein einziger Betrag darin steht. Das LfD-Schutzstufenkonzept nennt Sozialdaten ausdrücklich als Fall der Stufe D; § 35 SGB I stellt sie unter das Sozialgeheimnis.

Hinzu kommt, wen es trifft: Kinder, deren Bedürftigkeit in Schule, Verein und Mensa für Mitschüler sichtbar werden kann. Genau davor schützt die Einstufung.

Der Eigenanteil weist die Bezuschussung aus; die Teilnahmeliste liegt in der Einrichtung.
