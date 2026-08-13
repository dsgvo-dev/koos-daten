---
id: dstore-fiktionsbescheinigung
typ: datenspeicher
system: null
name: Fiktionsbescheinigung
datenkategorie: Migration & Aufenthalt
zuständige-einheit: oe-amt-47
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: AufenthG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-04'
tags:
- Fiktionsbescheinigung
- Aufenthalt
---


# Fiktionsbescheinigung

## Definition

Bescheinigung über die Fortgeltung eines Aufenthaltsstatus während eines laufenden Verfahrens.

## Felder

- Aktenzeichen
- Geltungsbeginn
- Geltungsende
- Nebenbestimmungen
- Ausstellende Behörde
- Person

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## Schutzstufe geprüft 2026-08-04

Durchsicht des Katalogs gegen das Schutzstufenkonzept des LfD Niedersachsen,
Maximalprinzip.

**Von C auf D.** Ein aufenthaltsrechtlicher Status entscheidet darüber, ob eine Person im Bundesgebiet bleiben darf. Das Schutzstufenkonzept ordnet der Stufe D Daten zu, deren Missbrauch die Existenz beeinträchtigen kann -- bei einer Aufenthaltsbeendigung ist das unmittelbar der Fall.

Hinzu kommt die faktische Wirkung: Der Aufenthaltsstatus wird gesellschaftlich als Merkmal der Herkunft gelesen, auch wenn er rechtlich keine Angabe über die ethnische Herkunft nach Art. 9 Abs. 1 DSGVO ist.

Die Fiktionsbescheinigung dokumentiert einen Schwebezustand: Der bisherige Status gilt fort, über den neuen ist nicht entschieden. Gerade diese Unsicherheit macht die Angabe für die betroffene Person heikel.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*
