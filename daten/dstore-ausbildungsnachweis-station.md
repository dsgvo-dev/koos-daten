---
id: dstore-ausbildungsnachweis-station
typ: datenspeicher
system: null
name: Ausbildungsnachweis und Stationszeugnis
datenkategorie: Recht & Compliance
zuständige-einheit: oe-amt-30
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
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. b
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: NDSG
    artikel: § 3
  - gesetz: NJAG
  - gesetz: NJAVO
  aufbewahrung:
    frist: 3 Jahre
    beginn: nach Übermittlung des Stationszeugnisses an das Landesjustizprüfungsamt
    hinweis: Festlegung des Trägers, angelehnt an die regelmäßige Verjährung nach
      § 195 BGB für etwaige Ansprüche aus der Ausbildung. Die eigentliche Ausbildungsakte
      führt das Landesjustizprüfungsamt nach dessen Aufbewahrungsregeln; die Ausbildungsstelle
      hält lediglich ein Doppel vor.
letzte-aktualisierung: '2026-08-10'
tags:
- Ausbildung
- Referendariat
- Stationszeugnis
---



# Ausbildungsnachweis und Stationszeugnis

## Definition

Unterlagen der Ausbildungsstelle über eine bei ihr abgeleistete Ausbildungsstation, insbesondere der Ausbildungsnachweis und das Stationszeugnis.

## Felder

- Name der auszubildenden Person
- Zuweisungszeitraum und Bezeichnung der Station
- ausbildende Person und Organisationseinheit
- Ausbildungsnachweis über Inhalte und bearbeitete Vorgänge
- Beurteilung und Stationszeugnis
- Datum der Übermittlung an das Landesjustizprüfungsamt

## Hinweise

Angelegt am 2026-07-30 zusammen mit `proc-referendarstation-durchfuehren` und `vvt-30-005`. `dstore-personalakte` passt nicht: Zwischen der Kommune und der auszubildenden Person besteht kein Personalverhältnis.

**Die Ausbildungsstelle ist nicht die aktenführende Stelle.** Das Ausbildungsverhältnis besteht zum Land; die Ausbildungsakte führt das Landesjustizprüfungsamt. Was hier vorgehalten wird, ist ein Doppel für Rückfragen -- daraus folgt die kurze Frist.

**Keine Klausur- und Arbeitsgemeinschaftsergebnisse.** Sie entstehen beim Oberlandesgericht, nicht bei der Ausbildungsstelle, und werden hier nicht geführt.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `hoch`** · **Verfügbarkeit: `normal`**

**Über `normal` gesetzt: Integrität `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

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

**Bleibt bei D.** **Beschäftigtendaten mit Bewertungsbezug.** Das LfD-Schutzstufenkonzept nennt dienstliche Beurteilungen ausdrücklich bei Stufe D. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Hinzu kommt das Abhängigkeitsverhältnis:** Beschäftigte können der Verarbeitung nicht ausweichen, und eine Offenlegung innerhalb der Verwaltung wirkt im täglichen Zusammenarbeiten fort. Für die Personalakte gilt zudem § 88 NBG mit einem eigenen Zugriffsregime, das strenger ist als das allgemeine Datenschutzrecht.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
