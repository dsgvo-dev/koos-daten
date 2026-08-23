---
id: dstore-bild-und-tonaufnahmen
typ: datenspeicher
system: null
name: Bild- und Tonaufnahmen
zuständige-einheit: oe-amt-10
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. a
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. e
  - gesetz: KUG
    artikel: §§ 22, 23
  - gesetz: NDSG
    artikel: § 3
  aufbewahrung:
    frist: bis zum Widerruf der Einwilligung; Archivgut nach NArchG dauerhaft
    beginn: mit der Aufnahme
    hinweis: Zweistufig. Aufnahmen erkennbar einzeln abgebildeter Personen beruhen
      auf Einwilligung und sind bei Widerruf aus künftigen Nutzungen zu entfernen.
      Übersichtsaufnahmen, auf denen Einzelne nur Beiwerk sind, beruhen auf § 3 NDSG
      und § 23 Abs. 1 Nr. 3 KUG.
letzte-aktualisierung: '2026-08-04'
tags:
- Bildaufnahme
- Tonaufnahme
- Öffentlichkeitsarbeit
- Einwilligung
---



# Bild- und Tonaufnahmen

## Definition

Foto-, Video- und Tonaufnahmen von Personen, die bei Veranstaltungen und Anlässen der
Verwaltung entstehen und für die Öffentlichkeitsarbeit, die Presse und das Bildarchiv
verwendet werden.

## Felder

- Aufnahme (Bild, Video, Ton)
- Anlass und Veranstaltung
- Aufnahmedatum und -ort
- abgebildete Person, soweit benannt
- Bildunterschrift
- Einwilligungsstatus und Datum der Einwilligung
- Widerrufsvermerk
- Verwendungszweck und erfolgte Veröffentlichungen
- Urheber beziehungsweise Fototeam

## Hinweise

Angelegt am 2026-07-29 zusammen mit `proc-kommunale-veranstaltung-planen-und-durchfuehren`
und `vvt-10-012`. Aufnahmen waren im Bestand als Datenart benannt, aber ohne eigenen
Datenspeicher geführt — obwohl für sie eine andere Aufbewahrungsregel gilt als für die
Anmeldedaten derselben Veranstaltung.

**Der Einwilligungsstatus ist ein Feld dieses Speichers, kein Beiwerk.** Ohne ihn lässt sich
ein Widerruf nicht umsetzen, weil nicht feststellbar ist, welche Aufnahmen betroffen sind.

**Zur dauerhaften Aufbewahrung:** Sie kommt nur für Aufnahmen in Betracht, die als Archivgut
nach dem Niedersächsischen Archivgesetz übernommen werden. Für alle übrigen endet die
Speicherung mit dem Widerruf der Einwilligung beziehungsweise dem Wegfall des
Verwendungszwecks.

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

## Schutzstufe geprüft 2026-08-14

**C bestätigt.** Die Aufnahme und ihr Kontext können die gesellschaftliche Stellung der
abgebildeten Person berühren; kein D, weil eine Veranstaltungsaufnahme keine biometrische
Verarbeitung ist. Der Einwilligungsstatus und der Widerrufsvermerk machen das Bild zu einem
verwalteten Vorgang.

Geprüft im Rahmen der Schutzstufendurchsicht Los 4 (Amt 10). Vorschlag:
`_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-14-los4-amt10.md`.

