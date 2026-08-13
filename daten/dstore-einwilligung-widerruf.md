---
id: dstore-einwilligung-widerruf
typ: datenspeicher
system: null
name: Einwilligung und Widerruf
datenkategorie: Verfahrensorganisation
zuständige-einheit: oe-amt-1-4
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
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. a
  - gesetz: DSGVO
    artikel: Art. 7
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. a
  aufbewahrung:
    frist: 3 Jahre
    beginn: nach Widerruf oder Wegfall des Zwecks
    hinweis: Nachweispflicht nach Art. 7 Abs. 1 DSGVO; angelehnt an die regelmäßige
      Verjährung nach § 195 BGB.
letzte-aktualisierung: '2026-08-10'
tags:
- Einwilligung
- Betroffenenrechte
- Art. 7 DSGVO
---


# Einwilligung und Widerruf

## Definition

Nachweis über eine erteilte Einwilligung und über ihren Widerruf, einschließlich der Unterrichtung, auf die sich die Einwilligung stützt.

## Felder

- Betroffene Person
- Gegenstand und Reichweite der Einwilligung
- Datum der Erteilung
- Form der Erteilung
- Nachweis der vorherigen Unterrichtung
- Datum des Widerrufs
- Umsetzung des Widerrufs mit Datum und ausführender Stelle

## Hinweise

Angelegt am 2026-08-03 zu `vvt-47-006` und `vvt-53-005`, verwendbar für alle Verarbeitungen auf Grundlage von Art. 6 Abs. 1 lit. a) oder Art. 9 Abs. 2 lit. a) DSGVO.

**Ohne diesen Speicher ist der Widerruf nicht umsetzbar.** Art. 7 Abs. 3 DSGVO gibt der betroffenen Person das Recht, die Einwilligung jederzeit zu widerrufen. Wird nirgends geführt, wer eingewilligt hat und ob widerrufen wurde, kann die Stelle weder den Widerruf vollziehen noch die Einwilligung nach Art. 7 Abs. 1 nachweisen.

Derselbe Befund war am 2026-07-30 bei `vvt-1-1-005` aufgetreten und dort über `dstore-bild-und-tonaufnahmen` gelöst worden. Dieser Speicher verallgemeinert die Lösung.

## Einstufung nach dem Maximalprinzip 2026-08-03

Die Schutzstufe richtet sich nach der sensibelsten Angabe, die in diesem Speicher anfallen **kann** -- nicht nach dem Regelfall. Ist die Verarbeitung von Daten nach Art. 9 Abs. 1 DSGVO möglich, gilt für den Speicher insgesamt die höhere Stufe.

Der Grund ist praktischer Natur: Technische und organisatorische Maßnahmen werden für den Speicher eingerichtet, nicht für den einzelnen Datensatz. Eine Einstufung, die erst im Einzelfall angehoben wird, führt zu Maßnahmen, die im Einzelfall nicht greifen.

**Von B auf D.** Das Feld „Gegenstand und Reichweite der Einwilligung" benennt, worin eingewilligt wurde. Bei `vvt-53-005` lautet der Gegenstand die Gesundheitsberatung, bei `vvt-47-006` die Übermittlung an Wohlfahrtsverbände im Asylkontext. Der Nachweis der Einwilligung offenbart damit dieselbe Information wie die Einwilligung selbst.

Das ist die unangenehme Folge eines übergreifenden Speichers: Er erbt die Schutzstufe der sensibelsten Verarbeitung, für die er geführt wird. Alternative wäre, je Fachbereich einen eigenen Einwilligungsnachweis zu führen -- das erhöht den Pflegeaufwand und wurde deshalb nicht gewählt.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** Die Einstufung wurde am 2026-08-04 bei der Anlage beziehungsweise
Überarbeitung dieses Speichers ausführlich begründet -- siehe die Hinweise oben. Der
Durchgang vom 2026-08-10 hat sie bestätigt und trägt hier nur den Prüfvermerk nach, der bisher
fehlte.

*Der Vermerk ist kein Formalismus: Ohne ihn zählte der Speicher als ungeprüft, und der
Rückstand wies 129 statt der tatsächlich offenen 115 Speicher aus -- allesamt auf Stufe C.*
