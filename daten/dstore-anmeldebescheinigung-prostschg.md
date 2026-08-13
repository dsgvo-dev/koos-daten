---
id: dstore-anmeldebescheinigung-prostschg
typ: datenspeicher
system: null
name: Anmeldebescheinigung und Aliasname nach ProstSchG
datenkategorie: Gesundheit & Erlaubnisse
zuständige-einheit: oe-amt-53
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: E
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: sehr hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: sehr hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. g
  - gesetz: NDSG
    artikel: § 17
  - gesetz: ProstSchG
    artikel: § 3
  - gesetz: ProstSchG
    artikel: § 5
  - gesetz: ProstSchG
    artikel: § 10
  aufbewahrung:
    frist: solange die Anmeldung gültig ist, längstens zwei Jahre
    beginn: nach Ablauf oder Widerruf der Anmeldung
    hinweis: '§ 34 Abs. 4 ProstSchG. Die kurze Frist ist Teil des Schutzkonzepts:
      jede über den Zweck hinausgehende Vorhaltung erhöht das Offenbarungsrisiko.'
letzte-aktualisierung: '2026-08-10'
tags:
- ProstSchG
- Art. 9 DSGVO
- Schutzstufe E
---



# Anmeldebescheinigung und Aliasname nach ProstSchG

## Definition

Anmeldebescheinigung nach § 5 ProstSchG einschließlich des auf Verlangen eingetragenen Aliasnamens, der die Ausübung der Tätigkeit gegenüber Dritten verbirgt.

## Felder

- Angemeldete Person
- Aliasname nach § 5 Abs. 6 ProstSchG
- Nummer und Gültigkeitsdauer der Anmeldebescheinigung
- Tätigkeitsorte nach § 4 ProstSchG
- Datum der Anmeldung und der Beratungsgespräche
- Widerruf oder Erlöschen

## Hinweise

Angelegt am 2026-08-03 zu `vvt-53-002` (Prostituiertenschutz).

**Erster Datenspeicher der Schutzstufe E.** Das Schutzstufenkonzept des LfD Niedersachsen sieht Stufe E vor, wenn unsachgemäße Handhabung Gesundheit, Leben oder Freiheit beeinträchtigen kann. Die Offenbarung der Tätigkeit als Prostituierte kann genau das auslösen. Der EuGH hat den Begriff der sensiblen Daten zum Sexualleben ausdrücklich weit gefasst (Urt. v. 02.12.2025, C-492/23).

**Der Aliasname ist selbst ein Schutzinstrument.** § 5 Abs. 6 ProstSchG lässt ihn zu, damit der bürgerliche Name nicht offenbart werden muss. Eine Datenart, die dem Schutz dient, muss selbst besonders geschützt werden -- die Zuordnung Alias zu bürgerlichem Namen ist der sensibelste Teil des gesamten Bestands.

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

**Bleibt bei E.** **Der Aliasname nach § 5 Abs. 6 ProstSchG ist der Beweis, dass der Gesetzgeber selbst von einer Gefährdung ausgeht.** Er existiert, damit die Tätigkeit gegenüber Dritten verborgen bleibt. Wird die Zuordnung von Alias und Klarnamen bekannt, ist der Schutz aufgehoben, den das Gesetz ausdrücklich schaffen wollte.

Betroffene sind häufig in Abhängigkeitsverhältnissen. Die Tätigkeitsorte nach § 4 ProstSchG machen sie auffindbar. § 34 ProstSchG stellt die Daten unter eine besondere Zweckbindung und verbietet die Weitergabe an Stellen, die nicht mit dem Vollzug des Gesetzes befasst sind.
