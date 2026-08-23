---
id: dstore-lebenslauf-qualifikationsnachweis
typ: datenspeicher
system: null
name: Lebenslauf und Qualifikationsnachweis
zuständige-einheit: oe-amt-11
bpmn:
  typ: datenobjekt
kontext:
  rolle: basis
  kontextabhaengig: true
  varianten:
  - id: dstore-lebenslauf-qualifikationsnachweis-vertraulich
    bedingung: verfahren-vertraulich
  regelquelle: regeln/kontextregeln.yaml
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: HeilprG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-10'
tags:
- Lebenslauf
- Qualifikation
- Zulassung
---


# Lebenslauf und Qualifikationsnachweis

## Definition

Angaben zum beruflichen Werdegang und zu Qualifikationen im Erlaubnisverfahren.

## Felder

- tabellarischer Lebenslauf
- Ausbildung
- Berufserfahrung
- Abschluss
- Nachweisdatei
- Prüfvermerk

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- HeilprG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Sektorale Heilpraktikererlaubnis für Physiotherapie

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Aufspaltung 2026-08-10: allgemeine und vertrauliche Variante

**Dieser Speicher deckt ab 2026-08-10 nur noch die Routineverfahren ab.** Der Qualifikationsnachweis in einer Fortbildungsliste und derselbe Lebenslauf in einem Bewerbungsverfahren.

Die Durchsicht der Allgemeinplätze hatte gezeigt, dass eine einzige Schutzstufe für diese
Datenart nicht tragfähig ist: Eine niedrige Stufe unterschätzt die vertraulichen Verfahren,
eine hohe belegt die Routineverfahren mit Maßnahmen, die sie nicht brauchen und die deshalb
in der Praxis unterlaufen werden.

Von den bisherigen 19 Verwendungen sind **4 auf `dstore-lebenslauf-qualifikationsnachweis-vertraulich`
(Stufe D) umgehängt** worden; 15 bleiben hier.

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
