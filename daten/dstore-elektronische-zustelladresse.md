---
id: dstore-elektronische-zustelladresse
typ: datenspeicher
system: null
name: Elektronische Zustelladresse
datenkategorie: Kontakt & Kommunikation
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenspeicher
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
  - gesetz: VwVfG
  - gesetz: EGovG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-12'
tags:
- E-Mail
- Postfach
- Zustellung
---


# Elektronische Zustelladresse

## Definition

Elektronische Adresse für behördliche Kommunikation und Zustellung.

## Felder

- E-Mail-Adresse
- De-Mail oder Postfach
- Einwilligung
- Zustellpräferenz
- Validierungsstatus
- Inhaber/in

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

**Herabgestuft von C auf B.** E-Mail-Adresse, De-Mail oder Postfach, Einwilligung,
Zustellpräferenz, Validierungsstatus.

Inhaltsgleich mit `dstore-kontaktdaten`, das seit dem 2026-08-10 geprüft auf B steht.

Wo die Kommunikationsdaten Schutzzweck haben, greift `dstore-kontaktdaten-vertraulich`
(Stufe D).

*Durchsicht Los 2 (Amt 33) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los2-amt33.md`.*
