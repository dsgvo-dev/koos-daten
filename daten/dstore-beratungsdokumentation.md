---
id: dstore-beratungsdokumentation
typ: datenspeicher
system: null
name: Beratungsdokumentation
datenkategorie: Kontakt & Kommunikation
zuständige-einheit: oe-amt-53
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
    artikel: Art. 6 Abs. 1 lit. a und lit. e
  - gesetz: NDSG
    artikel: § 3
  aufbewahrung:
    frist: 3 Jahre
    beginn: nach Abschluss der Beratung
    hinweis: Festlegung des Trägers, angelehnt an die regelmäßige Verjährung nach
      § 195 BGB.
letzte-aktualisierung: '2026-08-10'
tags:
- Beratung
- Dokumentation
---


# Beratungsdokumentation

## Definition

Dokumentation von Beratungsgesprächen ohne eigenes Verwaltungsverfahren: Anlass, Inhalt und Ergebnis der Beratung.

## Felder

- Ratsuchende Person
- Datum und Form der Beratung
- Anliegen
- Inhalt der Beratung
- Weiterverweisung
- beratende Fachkraft

## Hinweise

Angelegt am 2026-08-03 zu `vvt-51-006` (Fachberatung Kindertageseinrichtungen) und `vvt-53-005` (Gesundheitsberatung).

**Nur für Beratung ohne Gesundheitsbezug.** Enthält das Anliegen Gesundheitsdaten -- wie regelmäßig in der Gesundheitsberatung -- ist zusätzlich `dstore-gesundheitsdaten` zu führen und die Verarbeitung auf Art. 9 Abs. 2 zu stützen. Die einfache Einwilligung nach Art. 6 Abs. 1 lit. a) genügt dafür nicht.

Beruht die Beratung auf Einwilligung, ist `dstore-einwilligung-widerruf` mitzuführen.

## Einstufung nach dem Maximalprinzip 2026-08-03

Die Schutzstufe richtet sich nach der sensibelsten Angabe, die in diesem Speicher anfallen **kann** -- nicht nach dem Regelfall. Ist die Verarbeitung von Daten nach Art. 9 Abs. 1 DSGVO möglich, gilt für den Speicher insgesamt die höhere Stufe.

Der Grund ist praktischer Natur: Technische und organisatorische Maßnahmen werden für den Speicher eingerichtet, nicht für den einzelnen Datensatz. Eine Einstufung, die erst im Einzelfall angehoben wird, führt zu Maßnahmen, die im Einzelfall nicht greifen.

**Von C auf D.** Der Speicher führt das „Anliegen" einer Beratung. In der Gesundheitsberatung (`vvt-53-005`) ist das Anliegen regelmäßig ein Gesundheitsdatum, in der Gleichstellungsberatung kann es Gewaltbetroffenheit offenbaren. Der ursprüngliche Hinweis, bei Gesundheitsbezug sei zusätzlich `dstore-gesundheitsdaten` zu führen, bleibt richtig -- er ersetzt aber nicht die Einstufung dieses Speichers.

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
