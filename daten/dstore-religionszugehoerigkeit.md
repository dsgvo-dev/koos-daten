---
id: dstore-religionszugehoerigkeit
typ: datenspeicher
system: null
name: Religionszugehörigkeit
zuständige-einheit: oe-amt-40
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: sehr hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: sehr hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. g
  - gesetz: NDSG
    artikel: § 17
  - gesetz: NSchG
    artikel: § 63 Abs. 2
  aufbewahrung:
    frist: bis zum Ende der Grundschulzeit
    beginn: mit der Zuweisung zum Schulbezirk
    hinweis: Die Angabe ist nur zu speichern, solange die Zuweisung zu einer Bekenntnisschule
      sie erfordert. Entfällt dieser Zweck, ist sie unverzüglich zu löschen.
letzte-aktualisierung: '2026-08-10'
tags:
- Schule
- Art. 9 DSGVO
- Bekenntnisschule
---



# Religionszugehörigkeit

## Definition

Angabe über die Zugehörigkeit zu einer Religionsgemeinschaft, soweit sie für die Zuweisung zu einer Bekenntnisschule erforderlich ist.

## Felder

- Betroffene Person
- Religionsgemeinschaft
- Herkunft der Angabe (Elternangabe oder Melderegister)
- Datum der Erhebung

## Hinweise

Angelegt am 2026-08-03 zu `vvt-40-007` (Steuerung der Grundschulbezirke).

**Besonderes Datum nach Art. 9 Abs. 1 DSGVO.** Das Schutzstufenkonzept des LfD Niedersachsen ordnet solche Daten mindestens der Stufe D zu.

**OFFENE VORFRAGE — vor Nutzung zu klären.** Die Konfession ist für die Bezirkszuweisung nur erheblich, wenn im Gebiet Bekenntnisschulen bestehen. Trifft das nicht zu, ist die Datenart ersatzlos zu streichen; die hier eingetragene Rechtsgrundlage ersetzt diese Prüfung nicht.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `sehr hoch`** · **Verfügbarkeit: `normal`**

**Über `normal` gesetzt: Integrität `sehr hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Verfügbarkeit bleibt bei `normal`**, geprüft anhand der Fragen des Durchgangs vom 2026-08-04:

1. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

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
