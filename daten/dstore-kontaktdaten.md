---
id: dstore-kontaktdaten
typ: datenspeicher
system: null
name: Kontaktdaten
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
kontext:
  rolle: basis
  kontextabhaengig: true
  varianten:
  - id: dstore-kontaktdaten-vertraulich
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
- Kontakt
- Telefon
- E-Mail
konvertiert-aus: daten1/dtype-kontaktdaten.md
---


## Beschreibung

Kontaktinformationen einer Person oder Organisation: Telefon, E-Mail, Mobilnummer.

## Felder

- Telefonnummer
- Mobilnummer
- E-Mail-Adresse
- Faxnummer

## Rechtsgrundlage

Art. 6 DSGVO

## Löschfrist

Kontextabhängig

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

**Schutzstufe herabgesetzt 2026-08-04: D → B.** Die Erreichbarkeit einer Person —
Telefon, Mobilnummer, E-Mail, Fax — erfüllt für sich genommen das B-Kriterium des
LfD-Schutzstufenkonzepts: nicht frei zugänglich, ein Missbrauch beeinträchtigt die
Betroffenen nicht in ihrer gesellschaftlichen Stellung oder ihren wirtschaftlichen
Verhältnissen. Die vorige Einstufung D („streng vertraulich") war eine Voreinstellung
aus der Konvertierung (`daten1/dtype-kontaktdaten.md`), keine Bewertung.

**Grundsätzlich B — aber kontextabhängig höher. Dieser Speicher ist zu grob
geschnitten und muss aufgeteilt werden.** Er wird von 59 Verarbeitungstätigkeiten und
49 Prozessen geführt. In einem Teil dieser Verwendungen ist nicht die Nummer das
Schutzgut, sondern der Umstand, dass eine Person in diesem Verzeichnis überhaupt
geführt wird. Dasselbe Datum trägt dann eine höhere Stufe:

| Verarbeitungstätigkeit | was die Erreichbarkeit dort offenbart |
|

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-10

**Bleibt bei B.** **Identifikations- und interne Verwaltungsdaten.** Name, Kontaktdaten und der Nachweis, dass eine dienstliche Formalie erledigt ist. Die Angaben sind für die betroffene Person nicht belastend; ihre Preisgabe beeinträchtigt weder die gesellschaftliche Stellung noch die wirtschaftlichen Verhältnisse.

**Das gilt ausdrücklich nur für die Datenschutz-Schutzstufe.** Bei `dstore-it-berechtigungsantrag` und `dstore-schluesselverwaltung` liegt die Brisanz in der Informationssicherheit -- beide stehen dort seit dem 2026-08-04 auf hoher Integrität und hoher Verfügbarkeit. Die beiden Maßstäbe messen Verschiedenes, und das ist hier gut zu sehen.

*Sammelvermerk der Durchsicht vom 2026-08-10.*

## Aufspaltung 2026-08-10: allgemeine und vertrauliche Variante

**Dieser Speicher deckt ab 2026-08-10 nur noch die Routineverfahren ab.** Die Telefonnummer einer Gewerbetreibenden und die Handynummer einer Frau, die sich an die Gleichstellungsbeauftragte gewandt hat.

Die Durchsicht der Allgemeinplätze hatte gezeigt, dass eine einzige Schutzstufe für diese
Datenart nicht tragfähig ist: Eine niedrige Stufe unterschätzt die vertraulichen Verfahren,
eine hohe belegt die Routineverfahren mit Maßnahmen, die sie nicht brauchen und die deshalb
in der Praxis unterlaufen werden.

Von den bisherigen 63 Verwendungen sind **19 auf `dstore-kontaktdaten-vertraulich`
(Stufe D) umgehängt** worden; 44 bleiben hier.

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
