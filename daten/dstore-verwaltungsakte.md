---
id: dstore-verwaltungsakte
typ: datenspeicher
system: null
name: Verwaltungsakte
datenkategorie: Verwaltungsakte & Dokumente
zuständige-einheit: oe-amt-10
bpmn:
  typ: datenobjekt
kontext:
  rolle: basis
  kontextabhaengig: true
  varianten:
  - id: dstore-verwaltungsakte-vertraulich
    bedingung: verfahren-vertraulich
  regelquelle: regeln/kontextregeln.yaml
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
  - gesetz: NArchG
  - gesetz: NVwVfG
  aufbewahrung:
    frist: 10 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Akte
- Vorgang
- Aktenzeichen
konvertiert-aus: daten1/dtype-verwaltungsakte.md
---


## Beschreibung

Interne Vorgangsakte einer Behörde zu einem Verwaltungsvorgang.

## Felder

- Aktenzeichen
- Vorgangstitel
- Bearbeiter
- Erstellungsdatum
- Status
- Dokumente

## Rechtsgrundlage

NArchG, NVwVfG

## Löschfrist

10 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Die Aktenwahrheit und Aktenvollständigkeit ist ein hergebrachter Grundsatz des Verwaltungshandelns. Sie ist zugleich Voraussetzung für Akteneinsicht und gerichtliche Überprüfung.

## Aufspaltung 2026-08-10: allgemeine und vertrauliche Variante

**Dieser Speicher deckt ab 2026-08-10 nur noch die Routineverfahren ab.** Die Vorgangsakte zu einer Städtepartnerschaft und die Vorgangsakte zu einer Dienstaufsichtsbeschwerde.

Die Durchsicht der Allgemeinplätze hatte gezeigt, dass eine einzige Schutzstufe für diese
Datenart nicht tragfähig ist: Eine niedrige Stufe unterschätzt die vertraulichen Verfahren,
eine hohe belegt die Routineverfahren mit Maßnahmen, die sie nicht brauchen und die deshalb
in der Praxis unterlaufen werden.

Von den bisherigen 13 Verwendungen sind **5 auf `dstore-verwaltungsakte-vertraulich`
(Stufe D) umgehängt** worden; 8 bleiben hier.

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
