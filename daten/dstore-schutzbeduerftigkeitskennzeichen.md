---
id: dstore-schutzbeduerftigkeitskennzeichen
typ: datenspeicher
system: null
name: Schutzbedürftigkeitskennzeichen
datenkategorie: Bürgerdienste & Meldewesen
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
kontext:
  rolle: kontextanheber
  hebt-auf: E
  wirkung: >-
    Wo dieser Speicher gefuehrt wird, gilt fuer die Verarbeitung die Stufe E,
    unabhaengig von den uebrigen Speichern.
  regelquelle: regeln/kontextregeln.yaml
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: E
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: sehr hoch
  bsi-integritaet: sehr hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: sehr hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: DSGVO
    artikel: Art. 32 Abs. 1 lit. b
    titel: Vertraulichkeit der Systeme als technische Massnahme
  - gesetz: BMG
    artikel: § 51
    titel: Auskunftssperre bei Gefahr fuer Leben, Gesundheit, persoenliche Freiheit
  - gesetz: BMG
    artikel: § 52
    titel: Bedingter Sperrvermerk
  - gesetz: SGB VIII
    artikel: § 65
    titel: Besonderer Vertrauensschutz in der persoenlichen Beratung
  - gesetz: GewSchG
    artikel: § 1
    titel: Gerichtliche Schutzanordnungen
aufbewahrung:
    frist: Dauer der Gefaehrdungslage
    beginn: mit Eintragung
    hinweis: >-
      Die Auskunftssperre nach § 51 BMG ist auf zwei Jahre befristet und wird auf
      Antrag verlaengert. Das Kennzeichen ist mit Ablauf der Sperre zu ueberpruefen,
      nicht automatisch zu loeschen -- die Gefaehrdung endet nicht mit der Frist.
letzte-aktualisierung: '2026-08-10'
tags:
- Gewaltschutz
- Auskunftssperre
- Einzelfallschutz
---

# Schutzbedürftigkeitskennzeichen

## Definition

Kennzeichnung, dass für eine bestimmte Person eine Gefährdungslage besteht und Auskünfte,
Zustellungen und Rückrufe besonderen Vorkehrungen unterliegen. Das Kennzeichen sagt **nicht**,
worin die Gefährdung besteht.

## Felder

- Betroffene Person
- Art der Vorkehrung (keine Auskunft an Dritte, keine Zustellung an die Wohnanschrift, kein
  Rückruf ohne vorherige Ankündigung, Vorsprache nur nach Terminvereinbarung)
- Rechtsgrundlage oder Anlass der Eintragung
- Befristung und Wiedervorlage
- Eintragende Stelle und Datum
- Vermerk über jede Auskunft, die trotz Kennzeichen erteilt wurde, mit Grundlage

## Warum ein eigener Speicher und kein Feld

Die Gefährdung einer einzelnen Person lässt sich nicht über die Datenart abbilden. Zwei
Menschen, deren Anschrift in derselben Meldedatei steht, können sich in ihrer
Schutzbedürftigkeit vollständig unterscheiden -- die eine ist nach einer Trennung
untergetaucht, der andere hat gerade eine Wohnung gekauft. Die Schutzstufe bewertet die
Datenart, das Kennzeichen bewertet den Einzelfall. Beides ist nötig.

**Die Aufnahme in eine Verarbeitungstätigkeit hebt deren effektive Sensibilität an.** Wo
dieser Speicher geführt wird, ist die Verarbeitung mit den Maßnahmen der Stufe E zu
unterlegen, auch wenn die übrigen Speicher niedriger stehen.

## Was das Kennzeichen bewusst nicht enthält

**Es nennt den Grund nicht.** Das ist keine Nachlässigkeit, sondern die zentrale
Gestaltungsentscheidung.

Stünde im Kennzeichen „Gewaltschutzverfahren gegen den Ehemann" oder „Zeugin in einem
Strafverfahren", wäre die Kennzeichnung selbst die gefährlichste Angabe im Bestand -- und sie
müsste allen zugänglich sein, die eine Auskunft erteilen könnten, also praktisch dem gesamten
Bürgerservice. Das Kennzeichen wirkt nur, wenn es breit sichtbar ist; deshalb muss sein Inhalt
schmal sein.

Die sachbearbeitende Stelle, die den Hintergrund kennen muss, findet ihn im Fachverfahren.
Alle anderen brauchen nur die Handlungsanweisung.

## Anwendungsfälle

1. **Auskunftssperre nach § 51 BMG** -- Tatsachen begründen die Annahme einer Gefahr für Leben,
   Gesundheit, persönliche Freiheit oder ähnliche schutzwürdige Interessen. Die Sperre wirkt
   im Melderegister; das Kennzeichen trägt sie in die übrigen Fachverfahren.
2. **Bedingter Sperrvermerk nach § 52 BMG** -- bei Aufenthalt in einem Frauenhaus, einer
   Einrichtung der Jugendhilfe, einer Justizvollzugsanstalt oder einer psychiatrischen
   Einrichtung.
3. **Gerichtliche Schutzanordnung nach § 1 GewSchG** -- Näherungs- und Kontaktverbote setzen
   voraus, dass der Aufenthaltsort nicht bekannt wird.
4. **Kindeswohlschutz** -- nach einer Inobhutnahme nach § 42 SGB VIII darf der
   Unterbringungsort den Sorgeberechtigten unter Umständen nicht mitgeteilt werden.
5. **Zeugen- und Opferschutz** auf Ersuchen der Strafverfolgungsbehörden.

## Die eigentliche Schwachstelle: die Wirksamkeit

Ein Kennzeichen, das im Fachverfahren steht, aber beim Serienbrief nicht ausgewertet wird,
schützt niemanden. Drei Stellen sind zu prüfen:

- **Serienbriefe und Massenversand** -- Gebührenbescheide, Einladungen, Wahlbenachrichtigungen
  werden häufig aus einem Auszug erzeugt, in dem das Kennzeichen nicht mitgeführt wird.
- **Telefonische Auskunft** -- die häufigste Offenbarung geschieht mündlich und ohne Absicht.
  Die Auswertung muss dort erfolgen, wo der Datensatz aufgerufen wird, sichtbar und
  unübersehbar.
- **Übermittlung an andere Stellen** -- Melderegisterauskünfte, Auskünfte an Gerichte und
  Behörden, Statistikmeldungen.

Der Vermerk über erteilte Auskünfte trotz Kennzeichen ist deshalb Pflichtfeld: Er macht
nachvollziehbar, ob das Verfahren funktioniert.

## Schutzstufe geprüft 2026-08-10

**Stufe E.** Die Zuordnung ist unmittelbar: § 51 BMG setzt eine Gefahr für Leben, Gesundheit
oder persönliche Freiheit voraus -- das ist wörtlich der Tatbestand der höchsten Schutzstufe
des LfD-Konzepts. Wird das Kennzeichen missachtet oder wird bekannt, dass es besteht und für
wen, kann das den Schutz aufheben, dem es dient.

## BSI-Vektoren geprüft 2026-08-10

**Alle drei Vektoren erhöht -- ein seltener Fall, und hier begründet.**

- **Vertraulichkeit sehr hoch** -- schon die Existenz des Kennzeichens für eine bestimmte
  Person ist eine Information, die Verfolgern nützt.
- **Integrität sehr hoch** -- ein gelöschtes oder überschriebenes Kennzeichen führt dazu, dass
  Auskunft erteilt wird. Der Schaden entsteht nicht durch Verfälschung des Inhalts, sondern
  durch das Verschwinden des Eintrags. Jede Änderung ist deshalb zu protokollieren.
- **Verfügbarkeit hoch** -- steht das Kennzeichen im entscheidenden Moment nicht zur Verfügung,
  wirkt es nicht. Ein Ausfall darf nicht dazu führen, dass Auskünfte ungeprüft erteilt werden;
  die Fachverfahren sind so einzurichten, dass im Zweifel keine Auskunft ergeht.
