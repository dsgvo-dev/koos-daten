---
id: dstore-haftpflichtversicherung-hund
typ: datenspeicher
system: null
name: Haftpflichtversicherung Hund
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: NHundG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-12'
tags:
- Hund
- Versicherung
- Haftpflicht
---


# Haftpflichtversicherung Hund

## Definition

Versicherungsdaten zur Hundehalterhaftpflicht.

## Felder

- Versicherungsnehmer/in
- Versicherer
- Policennummer
- Deckungssumme
- Gültigkeit
- Hundebezug

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** Versicherungsnehmer/in, Versicherer, Policennummer, Deckungssumme, Gültigkeit.

**§ 5 NHundG** verlangt eine Haftpflichtversicherung. Der Speicher belegt, dass eine gesetzliche Pflicht erfüllt ist — mehr nicht. Die Deckungssumme ist gesetzlich vorgegeben und sagt nichts über die wirtschaftlichen Verhältnisse.

Die Haltung eines Hundes ist ein nach außen sichtbarer Alltagsvorgang. Für die *gewöhnliche* Hundehaltung trägt keine dieser Datenarten eine Beeinträchtigung der betroffenen Person.

**Abgrenzung.** `dstore-erlaubnis-gefaehrlicher-hund` und `dstore-maulkorb-leinenanordnung` bleiben bei C. Dort belegt der Eintrag einen ordnungsrechtlichen Vorgang gegen die Halterin — die Feststellung der Gefährlichkeit nach § 7 NHundG. Der Unterschied ist nicht der Hund, sondern der Verwaltungsakt.

**Lücke im Verzeichnis:** `verwendungen: 0`. Als eigener Auftrag vorgemerkt.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
