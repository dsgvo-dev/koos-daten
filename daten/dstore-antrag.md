---
id: dstore-antrag
typ: datenspeicher
system: null
name: Antrag
datenkategorie: Verwaltungsakte & Dokumente
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6
  - gesetz: NVwVfG
  aufbewahrung:
    frist: 5 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-12'
tags:
- Antrag
- Verwaltung
- Formular
konvertiert-aus: daten1/dtype-antrag.md
---


## Beschreibung

Allgemeiner Verwaltungsantrag eines Bürgers oder einer Organisation.

## Felder

- Antragsnummer
- Antragsdatum
- Antragsteller
- Antragsgegenstand
- Anlagen

## Rechtsgrundlage

Art. 6 DSGVO, NVwVfG

## Löschfrist

5 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-12

**Bleibt bei C.** Antragsnummer, Antragsdatum, Antragsteller, Antragsgegenstand, Anlagen.

Ein Behälter ohne festen Inhalt. `pruefung.py` führt diese Gruppe unter den generischen
Speichern (Regel R3: Zuordnung nur mit ausdrücklichem Beleg).

Der Bestand behandelt sie einheitlich auf C: `dstore-bescheid` C, `dstore-bescheinigung` C,
`dstore-verwaltungsakte` C — jeweils geprüft, letzterer mit einer Variante `-vertraulich`
auf D.

**C ist hier keine Verlegenheitslösung, sondern eine Aussage:** Der Behälter allein trägt
keine Einstufung; sie kommt von dem, was hineingelegt wird. Wo Sensibles hineingelegt wird,
steht die benannte Datenart daneben und trägt ihre eigene Stufe.

**`verwendungen: 0` ist hier kein Mangel.** Anders als bei den Hundespeichern aus Los 1
(Amt 32) ist das erwünscht: Ein generischer Behälter *soll* nicht gesetzt werden, wo eine
benannte Datenart passt.

*Durchsicht Los 2 (Amt 33) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los2-amt33.md`.*
