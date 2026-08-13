---
id: dstore-arbeitszeitaufzeichnung
typ: datenspeicher
system: null
name: Arbeitszeitaufzeichnung
datenkategorie: Personal
zuständige-einheit: oe-amt-11
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
    artikel: Art. 6 Abs. 1 lit. b und lit. c
  - gesetz: DSGVO
    artikel: Art. 88
  - gesetz: NDSG
    artikel: § 12
  - gesetz: NBG
    artikel: § 88
  - gesetz: ArbZG
    artikel: § 16 Abs. 2
  - gesetz: ArbSchG
    artikel: § 3 Abs. 2 Nr. 1
  - gesetz: NPersVG
    artikel: §§ 67, 78
  aufbewahrung:
    frist: 2 Jahre
    beginn: ab der Aufzeichnung
    hinweis: Frist aus § 16 Abs. 2 ArbZG und § 17 Abs. 2 MiLoG. Zeitdaten, die in
      die Lohn- und Gehaltsabrechnung eingehen, unterliegen als Buchungsbelege § 147
      AO und der NKomHKVO mit acht Jahren.
letzte-aktualisierung: '2026-08-04'
tags:
- Personal
- Arbeitszeit
- Zeiterfassung
- Beschäftigtendaten
---


# Arbeitszeitaufzeichnung

## Definition

Aufzeichnung der geleisteten Arbeitszeit der Beschäftigten im Zeitmanagementsystem, geführt zur Erfüllung der Aufzeichnungspflicht nach § 3 Abs. 2 Nr. 1 ArbSchG und § 16 Abs. 2 ArbZG.

## Felder

- Personalnummer und Name
- Organisationseinheit
- Kommt- und Gehtzeiten
- Pausenzeiten
- Zeitsaldo und Zeitausgleich
- Bereitschaftsdienst und Rufbereitschaft
- Anwesenheitsstatus
- Korrekturvermerke mit Grund und korrigierender Person

## Hinweise

Angelegt am 2026-07-30 zusammen mit `proc-arbeitszeit-erfassen-und-auswerten` und `vvt-11-004`.

**Abgrenzung zu `dstore-urlaubs-und-abwesenheitsdaten`.** Urlaub und sonstige Abwesenheiten werden dort geführt, weil für sie mit drei Jahren nach § 94 Abs. 2 Satz 1 NBG eine andere Frist gilt als für die Arbeitszeitaufzeichnung mit zwei Jahren nach § 16 Abs. 2 ArbZG. Beide Speicher werden im selben Fachverfahren gehalten, sind aber getrennt zu löschen.

**Der Anwesenheitsstatus ist ein eigenes Feld mit eigenem Empfängerkreis.** Empfang und Bürgerbüro benötigen für Auskünfte die Information, ob eine Person erreichbar ist — nicht deren Zeiten. Die Weitergabe ist eine Zweckänderung nach § 6 NDSG und auf diesen einen Wert begrenzt.

**Keine Gesundheitsdaten.** Krankheitsbedingte Abwesenheit wird ausschließlich als Abwesenheitsart und Dauer geführt. Diagnosen und ärztliche Bescheinigungen gehören nicht in diesen Speicher.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*
