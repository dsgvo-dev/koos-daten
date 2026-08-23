---
id: dstore-personalratsvorlage
typ: datenspeicher
system: null
name: Personalratsvorlage
zuständige-einheit: oe-amt-11
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
    artikel: Art. 6 Abs. 1 lit. c
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. b
  - gesetz: NDSG
    artikel: § 12
  - gesetz: NBG
    artikel: § 88
  - gesetz: NPersVG
    artikel: §§ 61, 65, 66, 67, 68
  aufbewahrung:
    frist: bis zum Abschluss des Beteiligungsverfahrens
    beginn: mit Übergabe der Vorlage an den Personalrat
    hinweis: Nach § 61 Abs. 1 NPersVG sind Unterlagen, die dem Personalrat aus Anlass
      seiner Beteiligung an einer bestimmten Maßnahme zur Verfügung gestellt wurden,
      nach Abschluss des Beteiligungsverfahrens an die Dienststelle zurückzugeben.
      Niederschriften und Personallisten des Personalrats unterliegen § 61 Abs. 2
      NPersVG.
letzte-aktualisierung: '2026-08-04'
tags:
- Personal
- Personalrat
- Mitbestimmung
- Beschäftigtendaten
---


# Personalratsvorlage

## Definition

Vorlage der Dienststelle an den Personalrat zu einer beteiligungspflichtigen Maßnahme, mit den für die Entscheidung erforderlichen Unterlagen.

## Felder

- Vorgangsnummer und Datum
- Mitbestimmungstatbestand mit Norm (§ 65, § 66 oder § 67 NPersVG)
- betroffene Person mit Name, Organisationseinheit und Funktion
- Sachverhaltsdarstellung
- beigefügte Unterlagen mit Angabe, welche Unterlage für welchen Tatbestand erforderlich ist
- Stellungnahme der Dienststelle
- Fristbeginn und Fristende des Beteiligungsverfahrens
- Beschluss des Personalrats und Datum
- Rückgabevermerk nach § 61 Abs. 1 NPersVG

## Hinweise

Angelegt am 2026-07-30 zusammen mit `proc-personalratsvorlage-erstellen-und-beteiligen` und `vvt-11-005`. Die Vorlage war im Bestand als Verarbeitung benannt, aber ohne eigenen Datenspeicher; `dstore-personalakte` und `dstore-bewerbungsunterlagen` treffen sie nicht, weil die Vorlage einen anderen Empfängerkreis und eine kürzere Lebensdauer hat.

**Der Rückgabevermerk ist ein Feld dieses Speichers, kein Beiwerk.** § 61 Abs. 1 NPersVG verlangt die Rückgabe an die Dienststelle nach Abschluss des Beteiligungsverfahrens. Ohne festgehaltenen Rückgabezeitpunkt ist nicht überprüfbar, ob die Pflicht erfüllt wurde.

**Die Angabe des Mitbestimmungstatbestands steuert den Umfang.** Welche Unterlagen beizufügen sind, richtet sich danach, worüber der Personalrat mitbestimmt. Deshalb wird je Unterlage festgehalten, für welchen Tatbestand sie erforderlich ist; die Personalakte als Ganzes wird nicht beigefügt.

## Schutzstufe geprüft 2026-08-04

Geprüft im Zuge der Auflösung von `vvt-61-001` und `vvt-61-002`: Alle Speicher mit
Freitextfeldern wurden gegen das Schutzstufenkonzept des LfD Niedersachsen gehalten.
Maßstab ist das Maximalprinzip -- die sensibelste Angabe, die anfallen **kann**.

Die entscheidende Frage lautet: **Schreibt die betroffene Person selbst hinein, oder
formuliert eine Fachstelle?** Ist der Text von außen frei bestimmbar, ist mit Angaben nach
Art. 9 Abs. 1 DSGVO zu rechnen. Formuliert eine Behörde sachbezogen, ist er es nicht.

**Von C auf D.** Der Speicher führt „Sachverhaltsdarstellung" und „Stellungnahme der Dienststelle" zu Maßnahmen nach §§ 65 ff. NPersVG -- Einstellung, Versetzung, Eingruppierung, Kündigung.

Solche Vorlagen stützen sich regelmäßig auf krankheitsbedingte Fehlzeiten, Schwerbehinderung, betriebliches Eingliederungsmanagement oder dienstliche Beurteilungen. Das Schutzstufenkonzept des LfD nennt **dienstliche Beurteilungen** ausdrücklich als Beispiel der Stufe D; Gesundheitsdaten ohnehin.

Hinzu kommt § 9 NPersVG: Die Mitglieder des Personalrats unterliegen einer besonderen Schweigepflicht. Eine Datenart, für die das Gesetz eine eigene Schweigepflicht anordnet, gehört nicht in die mittlere Schutzstufe.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*
