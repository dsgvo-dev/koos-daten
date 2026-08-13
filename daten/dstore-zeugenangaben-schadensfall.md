---
id: dstore-zeugenangaben-schadensfall
typ: datenspeicher
system: null
name: Zeugenangaben im Schadensfall
datenkategorie: Ordnung & Sicherheit
zuständige-einheit: oe-amt-86
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
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c, lit. e und lit. f
  - gesetz: BGB
    artikel: § 839
  - gesetz: GG
    artikel: Art. 34
  aufbewahrung:
    frist: 3 Jahre
    beginn: nach Abschluss des Schadensfalls
    hinweis: Regelmäßige Verjährung nach § 195 BGB; bei gerichtlicher Geltendmachung
      bis zum rechtskräftigen Abschluss.
letzte-aktualisierung: '2026-08-04'
tags:
- Zeugen
- Verkehrssicherung
- Schadensfall
---



# Zeugenangaben im Schadensfall

## Definition

Angaben von Personen, die einen Schaden an einer öffentlichen Straße oder dessen Verursachung beobachtet haben.

## Felder

- Zeugin oder Zeuge mit Name und Kontaktdaten
- Zeitpunkt und Ort der Beobachtung
- Sachverhaltsschilderung
- Bezug zum Schadensfall
- Einverständnis mit der Benennung gegenüber Dritten

## Hinweise

Angelegt am 2026-08-03 zu `vvt-86-001` (Anliegerpflichten und Verkehrssicherung), nach Auskunft des Fachamts vom 2026-08-03.

**Getrennt von der übrigen Schadensakte zu führen.** Zeuginnen und Zeugen haben regelmäßig kein Interesse daran, gegenüber der verursachenden Person benannt zu werden. Wird der Schaden zivilrechtlich weiterverfolgt, entsteht ein Interessenkonflikt zwischen dem Beweisinteresse der Kommune und dem Schutz der aussagenden Person. Das Feld zum Einverständnis mit der Benennung ist deshalb Teil des Speichers und nicht Beiwerk.

Zeuginnen und Zeugen sind über die Verarbeitung nach Art. 13 DSGVO zu unterrichten, insbesondere über eine mögliche Weitergabe an Versicherungen.

## Schutzstufe geprüft 2026-08-04

Geprüft im Zuge der Auflösung von `vvt-61-001` und `vvt-61-002`: Alle Speicher mit
Freitextfeldern wurden gegen das Schutzstufenkonzept des LfD Niedersachsen gehalten.
Maßstab ist das Maximalprinzip -- die sensibelste Angabe, die anfallen **kann**.

Die entscheidende Frage lautet: **Schreibt die betroffene Person selbst hinein, oder
formuliert eine Fachstelle?** Ist der Text von außen frei bestimmbar, ist mit Angaben nach
Art. 9 Abs. 1 DSGVO zu rechnen. Formuliert eine Behörde sachbezogen, ist er es nicht.

**Von C auf D.** Das Feld „Sachverhaltsschilderung" wird von der aussagenden Person frei formuliert und beschreibt regelmäßig Verletzungen und deren Folgen.

Hinzu kommt der Grund, aus dem der Speicher überhaupt getrennt geführt wird: Zeuginnen und Zeugen haben kein Interesse daran, gegenüber der verursachenden Person benannt zu werden. Wird die Zuordnung von Person und Aussage bekannt, kann das die aussagende Person unmittelbar betreffen. Eine Einstufung, die das nicht abbildet, widerspricht dem Zweck der Trennung.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `normal`** · **Verfügbarkeit: `hoch`**

**Über `normal` gesetzt: Verfügbarkeit `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Integrität bleibt bei `normal`**, geprüft anhand der Fragen des Durchgangs vom 2026-08-04:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

