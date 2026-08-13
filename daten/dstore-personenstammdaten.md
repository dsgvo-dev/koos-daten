---
id: dstore-personenstammdaten
typ: datenspeicher
system: null
name: Personenstammdaten
datenkategorie: Identitätsdaten
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
kontext:
  rolle: basis
  kontextabhaengig: true
  varianten:
  - id: dstore-personenstammdaten-vertraulich
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
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: PStG
  - gesetz: PStV
  - gesetz: BMG
  - gesetz: PAuswG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-10'
tags:
- Name
- Vorname
- Geburtsdatum
- Geburtsort
- Geschlecht
- Doktorgrad
---



# Personenstammdaten

## Definition

Grundlegende Identifikations- und Zuordnungsdaten natürlicher Personen, wie sie in Personenstands-, Melde- und Ausweisverfahren wiederkehrend verarbeitet werden.

## Felder

- Vorname
- Familienname
- früherer Name aus Eheschließung (Geburtsname)
  *Ein früherer Name nach Änderung des Geschlechtseintrags oder nach dem NamÄndG gehört
  nicht hierher, sondern in `dstore-frueherer-name-personenstandsaenderung` (Stufe E).*
- Geburtsdatum
- Geburtsort
- Geschlecht
- Doktorgrad

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- PStG
- PStV
- BMG
- PAuswG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Urkunde, Geburtsurkunde/Geburtenregister, Beantragung
- Eheschließung, Anmeldung
- Geburt, Anzeige
- Melderegisterauskunft, erweitert, Beantragung
- Personalausweis Beantragung
- Reisepass Beantragung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Zusammengeführt aus Personenstands-, Melde- und Identitätsverfahren; zentrale Basiskategorie ohne Spezialnachweise.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** Der Speicher wird in so vielen Verfahren geführt, dass ein Ausfall nicht ein Verfahren verzögert, sondern den Publikumsverkehr insgesamt zum Erliegen bringt. Das ist der Maßstab des BSI: erhebliche Beeinträchtigung der Aufgabenerfüllung.

Mit 175 Verwendungen der meistgenutzte Speicher des gesamten Bestands. Ohne ihn ist kein Verfahren durchführbar.

## Schutzstufe geprüft 2026-08-10

**D → C.** **Der meistgenutzte Speicher des Bestands stand auf der zweithöchsten Stufe -- und das war falsch.** 175 Verarbeitungen führen ihn; stünde er auf D, wäre praktisch jede Verarbeitung der Kommune eine D-Verarbeitung, und die Schutzstufe verlöre ihre Steuerungswirkung für die Maßnahmen nach Art. 32 DSGVO.

Der Inhalt trägt die Stufe nicht: Vorname, Familienname, Geburtsdatum, Geburtsort, Geschlecht, Doktorgrad. Keine dieser Angaben sagt etwas über Gesundheit, wirtschaftliche Verhältnisse oder Verhalten. **Stufe C und nicht B**, weil die Kombination aus Name, Geburtsdatum und Geburtsort der Schlüssel zu Identitätsmissbrauch ist und weil ein Geschlechtseintrag „divers" oder ein offengelassener Eintrag nach § 45b PStG für sich genommen aussagekräftig ist.

**Eine Angabe wurde ausgelagert.** Das Feld „frühere Namen" trug bisher die Last der Einstufung, weil ein früherer Vorname eine Änderung des Geschlechtseintrags offenbaren kann -- eine Angabe, deren Offenbarung § 13 SBGG untersagt und § 14 SBGG mit Bußgeld bedroht. Diese Konstellation ist selten, aber gravierend. Sie gehört nicht in den Speicher, der 175-fach verwendet wird, sondern in `dstore-frueherer-name-personenstandsaenderung` auf Stufe E.

**Die BSI-Werte bleiben unverändert hoch.** Integrität und Verfügbarkeit messen den Schaden für die Institution, nicht für die betroffene Person. Ein falscher oder nicht abrufbarer Stammdatensatz legt die Verwaltung lahm -- unabhängig davon, wie sensibel er ist. Der Fall zeigt die Trennung der beiden Maßstäbe besonders deutlich.

## Aufspaltung 2026-08-10: allgemeine und vertrauliche Variante

**Dieser Speicher deckt ab 2026-08-10 nur noch die Routineverfahren ab.** Der Name einer Person, die einen Bauantrag stellt, und der Name einer Person, die Grundsicherung bezieht -- dieselbe Datenart, ein anderer Aussagegehalt.

Die Durchsicht der Allgemeinplätze hatte gezeigt, dass eine einzige Schutzstufe für diese
Datenart nicht tragfähig ist: Eine niedrige Stufe unterschätzt die vertraulichen Verfahren,
eine hohe belegt die Routineverfahren mit Maßnahmen, die sie nicht brauchen und die deshalb
in der Praxis unterlaufen werden.

Von den bisherigen 175 Verwendungen sind **59 auf `dstore-personenstammdaten-vertraulich`
(Stufe D) umgehängt** worden; 116 bleiben hier.

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
