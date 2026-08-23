---
id: dstore-fundsache
typ: datenspeicher
system: null
name: Fundsache und Fundverwaltung
zuständige-einheit: oe-amt-33
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
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: BGB
    artikel: §§ 965-984
  - gesetz: NDSG
    artikel: § 3
  aufbewahrung:
    frist: 3 Jahre
    beginn: nach Rückgabe, Versteigerung oder Aneignung
    hinweis: Sechsmonatsfrist des § 973 BGB zuzüglich Rechtsbehelfs- und Prüfzeitraum;
      Festlegung des Trägers.
letzte-aktualisierung: '2026-08-12'
tags:
- Fundrecht
- Bürgerservice
---


# Fundsache und Fundverwaltung

## Definition

Angaben zu einer abgelieferten Fundsache sowie zu findender und verlierender Person.

## Felder

- Fundgegenstand mit Beschreibung
- Fundort und Funddatum
- findende Person mit Kontaktdaten
- verlierende oder empfangsberechtigte Person
- Wert bei Wertgegenständen
- Rückgabe mit Datum
- Finderlohn nach § 971 BGB
- Versteigerung oder Aneignung nach § 976 BGB

## Hinweise

Angelegt am 2026-08-03 zu `vvt-33-004` (Fundsachen-Verwaltung im Bürgerservice).

**Abgrenzung zu `dstore-verwahrgut-sicherstellung`.** Dieser betrifft Gegenstände, die nach §§ 26, 27 NPOG hoheitlich sichergestellt und verwahrt werden -- also gegen den Willen der betroffenen Person. Die Fundsache gelangt dagegen freiwillig in die Verwahrung, und die Rechtsbeziehungen richten sich nach §§ 965 ff. BGB.

**Der Gegenstand selbst kann personenbezogen sein.** Eine gefundene Brieftasche, ein Mobiltelefon oder ein Terminkalender enthalten Daten der verlierenden Person, die die Fundbehörde zwangsläufig zur Kenntnis nimmt, wenn sie den Eigentümer ermitteln will. Die Einsichtnahme ist auf das zur Ermittlung Erforderliche zu beschränken.

**Der Finderlohn führt zu einer Zahlungsbeziehung** zwischen findender und verlierender Person; die Behörde vermittelt sie und speichert dafür beide Namen.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** Fundgegenstand, Fundort und Funddatum, findende Person,
verlierende Person, Wert, Rückgabe, Finderlohn nach § 971 BGB, Versteigerung oder Aneignung
nach § 976 BGB.

Ein Fund ist ein Alltagsvorgang. Dass jemand einen Schirm verloren oder eine Geldbörse
abgegeben hat, sagt über ihn nichts Nachteiliges.

Das Feld „Wert" bezeichnet den Wert der **Sache**, nicht das Vermögen der Person. Es trägt
deshalb keine Aussage über die wirtschaftlichen Verhältnisse.

*Durchsicht Los 2 (Amt 33) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los2-amt33.md`.*
