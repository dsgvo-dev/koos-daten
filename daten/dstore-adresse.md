---
id: dstore-adresse
typ: datenspeicher
system: null
name: Adresse
datenkategorie: Person & Identität
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
kontext:
  rolle: basis
  kontextabhaengig: true
  varianten:
  - id: dstore-adresse-vertraulich
    bedingung: verfahren-vertraulich
  regelquelle: regeln/kontextregeln.yaml
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6
  aufbewahrung:
    frist: Kontextabhängig
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Adresse
- Anschrift
- Wohnort
konvertiert-aus: daten1/dtype-adresse.md
---


## Beschreibung

Wohn- oder Geschäftsadresse: Straße, Hausnummer, PLZ, Ort.

## Felder

- Straße
- Hausnummer
- Adresszusatz
- Postleitzahl
- Ort
- Land

## Rechtsgrundlage

Art. 6 DSGVO

## Löschfrist

Kontextabhängig

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

**Schutzstufe herabgesetzt 2026-08-04: D → B.** Die Anschrift für sich genommen
erfüllt das B-Kriterium des LfD-Schutzstufenkonzepts — nicht frei zugänglich, ein
Missbrauch beeinträchtigt die Betroffenen nicht in ihrer gesellschaftlichen Stellung
oder ihren wirtschaftlichen Verhältnissen. Die vorige Einstufung D („streng
vertraulich") war eine Voreinstellung aus der Konvertierung
(`daten1/dtype-adresse.md`), keine Bewertung.

Nicht A: Eine Wohnanschrift wird von den Betroffenen gerade nicht frei zugänglich
gemacht. Das Melderecht schützt sie ausdrücklich — Auskunftssperre nach § 51 BMG und
Übermittlungssperre nach § 36 BMG. Für diese Sperren bestehen eigene Speicher
(`dstore-auskunftssperre-melderegister`, Stufe E, und
`dstore-uebermittlungssperre-melderegister`, Stufe C); sie tragen die
Schutzbedürftigkeit des Einzelfalls, nicht dieser Speicher.

Geprüft wurden alle vier Verarbeitungstätigkeiten, die diesen Speicher führen:
`vvt-10-020` (Kontaktdaten allgemein), `vvt-33-001` (Melderegisterführung),
`vvt-40-008` (Schulraumvermietung), `vvt-40-009` (Beschaffung Schulausstattung).
Keine davon verarbeitet über die Anschrift eine sensible Angabe, und alle vier
führen keine besonderen Kategorien allein über dieses Datum. Das Maximalprinzip
nach R6 führt daher nicht zu einer höheren Stufe.

Abgrenzung: Adressdaten mit melderechtlichem Statusbezug gehören nicht hierher,
sondern nach `dstore-meldeadresse-wohnsitz`, `dstore-wohnstatus-haupt-nebenwohnung`
oder `dstore-meldedaten`.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Aufspaltung 2026-08-10: allgemeine und vertrauliche Variante

**Dieser Speicher deckt ab 2026-08-10 nur noch die Routineverfahren ab.** Die Anschrift eines Grundstücks und die Anschrift einer Gemeinschaftsunterkunft.

Die Durchsicht der Allgemeinplätze hatte gezeigt, dass eine einzige Schutzstufe für diese
Datenart nicht tragfähig ist: Eine niedrige Stufe unterschätzt die vertraulichen Verfahren,
eine hohe belegt die Routineverfahren mit Maßnahmen, die sie nicht brauchen und die deshalb
in der Praxis unterlaufen werden.

Von den bisherigen 29 Verwendungen sind **8 auf `dstore-adresse-vertraulich`
(Stufe D) umgehängt** worden; 21 bleiben hier.

**Zuordnungsregel.** Maßgeblich ist eine einzige Frage:

> *Wäre es für die betroffene Person nachteilig, wenn bekannt würde, dass sie in diesem
> Verfahren geführt wird?*

Wird sie bejaht, gehört die Verarbeitung zur vertraulichen Variante. Das war bei 63 der 221
aktiven Verarbeitungen der Fall -- Sozialhilfe, Jugendhilfe, Sozialpsychiatrie,
Eingliederungshilfe, Aufenthaltsrecht, Gesundheitsamt, Bußgeld- und Vollstreckungsverfahren,
Bewerbungsverfahren, Beratungsangebote und Beschwerdeverfahren.

Nicht ausschlaggebend war, ob die Verarbeitung *irgendeinen* Speicher der Stufe D führt: Ein
Führungszeugnis in einem Gewerbeerlaubnisverfahren macht die Gewerbeanmeldung nicht
vertraulich, denn die Anmeldung selbst ist ein öffentlicher Vorgang.

**Einzelfallschutz bleibt eine eigene Frage.** Dass eine bestimmte Person untergetaucht ist
oder unter Zeugenschutz steht, lässt sich über die Datenart nicht abbilden. Dafür gibt es seit
dem 2026-08-10 `dstore-schutzbeduerftigkeitskennzeichen` auf Stufe E.
