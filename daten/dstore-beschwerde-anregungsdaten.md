---
id: dstore-beschwerde-anregungsdaten
typ: datenspeicher
system: null
name: Beschwerde- und Anregungsdaten
datenkategorie: Bürgerbeteiligung & Service
zuständige-einheit: oe-amt-33
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
  - gesetz: NKomVG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-04'
tags:
- Beschwerde
- Anregung
- Lob
- Kritik
---



# Beschwerde- und Anregungsdaten

## Definition

Daten zu Eingaben, Beschwerden, Lob oder Anregungen an die Verwaltung.

## Felder

- Eingebende Person
- Kontakt
- Anliegen
- Sachgebiet
- Datum
- Rückmeldewunsch

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## Schutzstufe geprüft 2026-08-04

Geprüft im Zuge der Auflösung von `vvt-61-001` und `vvt-61-002`: Alle Speicher mit
Freitextfeldern wurden gegen das Schutzstufenkonzept des LfD Niedersachsen gehalten.
Maßstab ist das Maximalprinzip -- die sensibelste Angabe, die anfallen **kann**.

Die entscheidende Frage lautet: **Schreibt die betroffene Person selbst hinein, oder
formuliert eine Fachstelle?** Ist der Text von außen frei bestimmbar, ist mit Angaben nach
Art. 9 Abs. 1 DSGVO zu rechnen. Formuliert eine Behörde sachbezogen, ist er es nicht.

**Von C auf D.** Der Speicher führt das Feld „Anliegen" und wird in zehn Verarbeitungstätigkeiten verwendet -- darunter die Beratung der Gleichstellungsbeauftragten (`vvt-1-2-001`), Dienstaufsichtsbeschwerden (`vvt-11-007`) sowie Beschwerden und Petitionen (`vvt-1-1-002`).

Was eine Bürgerin in ein Beschwerdefeld schreibt, bestimmt sie selbst. Bei der Gleichstellungsberatung ist die Schilderung häuslicher Gewalt der Anlass des Angebots, nicht sein Randfall; bei einer Dienstaufsichtsbeschwerde werden regelmäßig gesundheitliche oder familiäre Umstände vorgetragen, um das Verhalten einer Beschäftigten einzuordnen.

**Der Speicher erbt die Schutzstufe der sensibelsten Verwendung.** Das ist die Folge eines übergreifenden Speichers; die Alternative wäre, je Fachbereich einen eigenen Beschwerdespeicher zu führen, was den Pflegeaufwand erhöht, ohne die Sache zu verbessern.

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

