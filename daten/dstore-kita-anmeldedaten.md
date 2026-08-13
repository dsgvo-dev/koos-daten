---
id: dstore-kita-anmeldedaten
typ: datenspeicher
system: null
name: Kita-Anmeldedaten
datenkategorie: Jugend & Betreuung
zuständige-einheit: oe-amt-51
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
  - gesetz: SGB VIII
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Kita
- Anmeldung
- Betreuung
---


# Kita-Anmeldedaten

## Definition

Anmeldedaten für einen Betreuungsplatz in Kindertagesstätte oder Tagespflege.

## Felder

- Kind
- Sorgeberechtigte
- Betreuungswunsch
- Betreuungsumfang
- Wunscheinrichtung
- Startdatum

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

**Bleibt bei C.** Kind, Sorgeberechtigte, Betreuungswunsch und Umfang. Der Betreuungsumfang lässt auf die Erwerbstätigkeit der Eltern schließen -- das trägt Stufe C, mehr nicht.

**Die Abgrenzung ist wichtiger als die Stufe:** Sobald bei der Anmeldung Allergien, Medikamente, ein Integrationsbedarf oder eine Eingliederungshilfe nach § 35a SGB VIII erfasst werden, sind das Gesundheitsdaten nach Art. 9 DSGVO. Sie gehören nicht in diesen Speicher, sondern in einen eigenen auf Stufe D. Das Anmeldeformular ist daraufhin zu prüfen.
