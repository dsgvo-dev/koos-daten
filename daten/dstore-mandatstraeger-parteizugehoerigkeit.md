---
id: dstore-mandatstraeger-parteizugehoerigkeit
typ: datenspeicher
system: null
name: Politische Zugehörigkeit von Mandatsträgern
datenkategorie: Wahlen & Gremien
zuständige-einheit: oe-amt-10
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
    artikel: Art. 9 Abs. 2 lit. e
  - gesetz: NDSG
    artikel: § 17
  - gesetz: NKomVG
    artikel: § 57
  aufbewahrung:
    frist: dauerhaft als Archivgut
    beginn: nach Ende der Wahlperiode
    hinweis: Sitzungsunterlagen der Vertretung werden nach § 3 NArchG dem Archiv angeboten.
letzte-aktualisierung: '2026-08-10'
tags:
- Ratsinformation
- Art. 9 DSGVO
- Mandat
---



# Politische Zugehörigkeit von Mandatsträgern

## Definition

Angaben zur Fraktions-, Gruppen- oder Parteizugehörigkeit von Mitgliedern der Vertretung und ihrer Ausschüsse.

## Felder

- Mandatsträgerin oder Mandatsträger
- Fraktion oder Gruppe
- Parteizugehörigkeit
- Beginn und Ende der Zugehörigkeit
- Funktion in Fraktion oder Ausschuss

## Hinweise

Angelegt am 2026-08-03 zu `vvt-10-014` (Sitzungsmanagement der Vertretung).

**Besonderes Datum nach Art. 9 Abs. 1 DSGVO** -- politische Meinung. Die VVT stützt sich auf Art. 9 Abs. 2 lit. e) DSGVO, also darauf, dass die betroffene Person die Daten offensichtlich öffentlich gemacht hat.

**Das trägt nicht für alle Betroffenen gleich weit.** Bei gewählten Mitgliedern der Vertretung ist die Fraktionszugehörigkeit öffentlich und der Erlaubnistatbestand greift. Bei **sachkundigen Bürgerinnen und Bürgern in Ausschüssen** ist eine Parteinähe nicht notwendig öffentlich gemacht; für sie ist die Grundlage gesondert zu prüfen. Das ist bei der Führung dieses Speichers zu unterscheiden.

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

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Gesundheit und andere besondere Kategorien nach Art. 9 DSGVO.** Die Verarbeitung ist grundsätzlich untersagt und nur zulässig, wenn ein Ausnahmetatbestand des Art. 9 Abs. 2 DSGVO greift. Das LfD-Schutzstufenkonzept ordnet diese Angaben der Stufe D zu; die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Praktische Folge:** Für diese Speicher ist der Zugriff auf die Personen zu beschränken, die ihn zur Aufgabenerfüllung brauchen -- eine amtsärztliche Stellungnahme gehört nicht in die allgemeine Personalakte, sondern in einen gesondert geführten Teilbestand.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
