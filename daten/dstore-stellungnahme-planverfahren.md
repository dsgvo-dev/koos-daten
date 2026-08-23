---
id: dstore-stellungnahme-planverfahren
typ: datenspeicher
system: null
name: Stellungnahme im Planverfahren
zuständige-einheit: oe-amt-61
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: BauGB
    artikel: § 3 Abs. 2
    titel: Beteiligung der Öffentlichkeit, Prüf- und Mitteilungspflicht
  - gesetz: BauGB
    artikel: § 1 Abs. 7
    titel: Abwägungsgebot
  - gesetz: NDSG
    artikel: § 17
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Bestandskraft des Plans
    hinweis: >-
      Bei anhängigem Normenkontroll- oder Rechtsbehelfsverfahren bis zu dessen
      rechtskräftigem Abschluss. Der Plan selbst wird nach § 3 NArchG dauerhaft
      archiviert; die Stellungnahmen einzelner Personen teilen diese Frist nicht.
letzte-aktualisierung: '2026-08-10'
tags:
- Bauleitplanung
- Öffentlichkeitsbeteiligung
- Freitext
---

# Stellungnahme im Planverfahren

## Definition

Von Bürgerinnen und Bürgern abgegebene Stellungnahmen und Anregungen zu Bauleitplänen und
anderen planerischen Vorhaben, einschließlich der Prüfung durch die Gemeinde und der
Mitteilung des Ergebnisses.

## Felder

- Stellungnehmende Person mit Name und Anschrift
- Kontaktdaten für die Mitteilung des Prüfergebnisses
- Bezug zum Plan oder Vorhaben
- Wortlaut der Stellungnahme
- Betroffenheit (Grundstücksbezug, Nachbarschaft, sonstiges Interesse)
- Eingangsdatum und Fristwahrung
- Prüfergebnis und Abwägungsvermerk
- Mitteilung des Ergebnisses mit Datum
- Kennzeichnung für die öffentliche Ratsvorlage

## Hinweise

Angelegt am 2026-08-04 zu `vvt-61-001` (Bauleitplanung und Öffentlichkeitsbeteiligung) und
`vvt-61-002` (Planerische Stellungnahmen und Bürgereingaben).

**Die Datenart ist unvermeidbar — das unterscheidet sie von Chatbot und Portal-Upload.**

Bei einem Chatbot oder einem Upload-Feld kann die Verantwortliche den Kanal gestalten: Sie
kann das Feld begrenzen, auf sensible Angaben hinweisen oder es weglassen. Am 2026-08-03 war
das die richtige Antwort, und bei den Menüpräferenzen einer Veranstaltung hat der Träger sie
gewählt: Eine Datenart nicht zu erheben ist wirksamer, als sie zu erheben und besonders zu
schützen.

**Hier geht das nicht.** § 3 Abs. 2 Satz 6 BauGB bestimmt: „Die fristgemäß abgegebenen
Stellungnahmen sind zu prüfen; das Ergebnis ist mitzuteilen." Die Gemeinde muss jede
fristgemäße Stellungnahme entgegennehmen, prüfen und beantworten. Eine Zeichenbegrenzung,
ein Ausschluss von Freitext oder ein Formularzwang würden das Beteiligungsrecht verkürzen
und wären rechtswidrig. Das Abwägungsgebot des § 1 Abs. 7 BauGB verlangt zudem, dass der
Vortrag inhaltlich erfasst wird — nicht nur seine Kategorie.

Damit greift das Maximalprinzip ohne Ausweichmöglichkeit: Was in einer Stellungnahme steht,
reicht von der sachlichen Einwendung bis zur Schilderung einer Erkrankung, die durch
Lärmimmissionen verschlimmert wird, oder einer politischen Überzeugung zum Vorhaben. Stufe
D.

**Der Schutz muss deshalb am anderen Ende ansetzen — bei der Weitergabe.**

Zwei gesetzlich angeordnete Offenlegungen sind zu bedenken:

1. **§ 3 Abs. 2 Satz 8 BauGB** — bei der Vorlage des Plans nach § 6 oder § 10 Abs. 2 sind
   die **nicht berücksichtigten Stellungnahmen** mit einer Stellungnahme der Gemeinde
   beizufügen. Sie gehen damit an die höhere Verwaltungsbehörde. Das ist eine
   Pflichtübermittlung, keine Ermessensentscheidung.
2. **Die Abwägung geht in die Ratsvorlage**, und Sitzungen der Vertretung sind nach § 64
   NKomVG grundsätzlich öffentlich. Ohne Vorkehrung erscheinen Name und Anliegen einzelner
   Personen in allgemein zugänglichen Sitzungsunterlagen und im Ratsinformationssystem.

Für den zweiten Fall ist die **Pseudonymisierung in der Abwägungstabelle** der wirksame
Schutz: In der öffentlichen Vorlage werden die Einwendungen laufend nummeriert, die
Zuordnung zur Person bleibt in der Verwaltungsakte. Das Feld „Kennzeichnung für die
öffentliche Ratsvorlage" hält fest, welche Nummer welcher Stellungnahme zugeordnet ist.

**Nicht die Eingabe begrenzen, sondern die Veröffentlichung.** Das ist die Umkehrung des
sonst richtigen Grundsatzes und folgt daraus, dass hier ein Beteiligungsrecht ausgeübt wird.

**Sonderfall § 3 Abs. 2 Satz 7 BauGB.** Haben mehr als 50 Personen inhaltsgleiche
Stellungnahmen abgegeben, kann die Einzelmitteilung durch eine öffentlich bekanntgemachte
Einsichtsmöglichkeit ersetzt werden. Dann werden zwar weniger Mitteilungen versandt, die
Namen aber weiterhin geführt — die Erleichterung betrifft das Verfahren, nicht die
Datenverarbeitung.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `hoch`** · **Verfügbarkeit: `hoch`**

**Über `normal` gesetzt: Integrität `hoch` und Verfügbarkeit `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** Die Einstufung wurde am 2026-08-04 bei der Anlage beziehungsweise
Überarbeitung dieses Speichers ausführlich begründet -- siehe die Hinweise oben. Der
Durchgang vom 2026-08-10 hat sie bestätigt und trägt hier nur den Prüfvermerk nach, der bisher
fehlte.

*Der Vermerk ist kein Formalismus: Ohne ihn zählte der Speicher als ungeprüft, und der
Rückstand wies 129 statt der tatsächlich offenen 115 Speicher aus -- allesamt auf Stufe C.*
