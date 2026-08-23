---
id: dstore-frueherer-name-personenstandsaenderung
typ: datenspeicher
system: null
name: Früherer Name nach Personenstands- oder Geschlechtseintragsänderung
zuständige-einheit: oe-amt-33
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
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: sehr hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. g
    titel: erhebliches oeffentliches Interesse, soweit Rueckschluesse auf Gesundheitsdaten moeglich sind
  - gesetz: SBGG
    artikel: § 13
    titel: Offenbarungsverbot
  - gesetz: SBGG
    artikel: § 14
    titel: Bussgeldvorschrift
  - gesetz: TSG
    artikel: § 5
    titel: Offenbarungsverbot fuer Altfaelle
  - gesetz: PStG
    artikel: § 45b
    titel: Aenderung der Geschlechtsangabe bei Varianten der Geschlechtsentwicklung
  - gesetz: NamAendG
    artikel: § 3
    titel: Aenderung des Namens aus wichtigem Grund
  aufbewahrung:
    frist: nach den Fristen des jeweiligen Fachverfahrens
    beginn: mit Abschluss des Verfahrens
    hinweis: >-
      Der frühere Name ist zu löschen, sobald das Verfahren ihn nicht mehr benötigt.
      Eine Vorhaltung "für alle Fälle" ist unzulässig, weil sie das Offenbarungsrisiko
      ohne Zweck aufrechterhält.
letzte-aktualisierung: '2026-08-10'
tags:
- Selbstbestimmungsgesetz
- Offenbarungsverbot
- Gewaltschutz
---

# Früherer Name nach Personenstands- oder Geschlechtseintragsänderung

## Definition

Der vor einer Namens- oder Geschlechtseintragsänderung geführte Name einer Person sowie die
Verknüpfung dieses Namens mit dem heutigen Namen. Ausgegliedert aus
`dstore-personenstammdaten` am 2026-08-10.

## Felder

- Früher geführter Vorname
- Früher geführter Familienname, soweit die Änderung nicht auf Eheschließung beruht
- Rechtsgrund der Änderung (Erklärung nach dem SBGG, Beschluss nach dem TSG, Änderung
  nach § 45b PStG, Namensänderung nach dem NamÄndG)
- Datum der Wirksamkeit
- Verknüpfung zum heutigen Namen
- Vermerk über jede Offenbarung mit Datum, Anlass und Rechtsgrundlage

## Abgrenzung

**Der Regelfall gehört nicht hierher.** Ein Geburtsname, der durch Eheschließung abgelegt
wurde, ist eine gewöhnliche Angabe und bleibt in `dstore-personenstammdaten` auf Stufe C.
Dieser Speicher erfasst die Fälle, in denen der frühere Name selbst die schutzbedürftige
Information ist.

## Hinweise

**Warum Stufe E und nicht D.** Die Stufe E ist Angaben vorbehalten, deren Offenbarung Leben,
Gesundheit oder Freiheit gefährden kann. Hier ist das keine Prognose der Verwaltung, sondern
die Wertung des Gesetzgebers:

- **§ 13 Abs. 1 SBGG** verbietet es, den früheren Vornamen oder den früheren Geschlechtseintrag
  ohne Zustimmung der betroffenen Person zu offenbaren oder auszuforschen. **§ 14 SBGG** stellt
  den Verstoß unter Bußgeld bis 10.000 Euro. Für Altfälle gilt § 5 TSG unverändert fort.
- Ein Gesetzgeber, der eine Offenbarung mit Bußgeld bedroht, hält sie für gefährlich. Das ist
  sie auch: Die Zwangsoutung transgeschlechtlicher Menschen führt zu Diskriminierung am
  Arbeitsplatz, im Wohnungsmarkt und zu Gewalt.
- Aus dem früheren Vornamen und dem heutigen Geschlechtseintrag lassen sich zudem
  **Gesundheitsdaten nach Art. 9 DSGVO** erschließen, ohne dass eine Diagnose genannt wird.

**Der zweite Fall: Namensänderung aus Gewaltschutzgründen.** Eine Änderung nach § 3 NamÄndG
wird unter anderem bewilligt, wenn eine Person sich vor einem Verfolger verbergen muss. Wird
die Verknüpfung von altem und neuem Namen bekannt, ist der gesamte Schutz aufgehoben. Diese
Fälle laufen regelmäßig parallel zu einer Auskunftssperre nach § 51 BMG -- siehe
`dstore-auskunftssperre-melderegister`, ebenfalls Stufe E.

**Praktische Folgen für die Fachverfahren.** Drei Punkte sind zu prüfen:

1. **Historisierung.** Fachverfahren führen Namensänderungen üblicherweise als Historie mit,
   die jeder Sachbearbeitung angezeigt wird. Genau das ist der Offenbarungstatbestand des
   § 13 SBGG. Die Historie muss in diesen Fällen zugriffsbeschränkt sein.
2. **Altbestände.** Aktenzeichen, Dateinamen, Verteiler und Serienbriefvorlagen führen den
   alten Namen oft weiter, ohne dass es jemandem auffällt.
3. **Auskünfte.** Vor jeder Auskunft an Dritte ist zu prüfen, ob eine Änderung nach dem SBGG,
   dem TSG oder dem NamÄndG vorliegt. Der Offenbarungsvermerk hält fest, wann dennoch
   offenbart wurde und auf welcher Grundlage -- § 13 Abs. 2 SBGG lässt Ausnahmen nur eng zu.

## Schutzstufe geprüft 2026-08-10

Angelegt im Rahmen der Schutzstufendurchsicht. Anlass war die Herabstufung von
`dstore-personenstammdaten` von D auf C: Das Feld "frühere Namen" trug dort allein die hohe
Einstufung eines Speichers, der in 175 Verarbeitungen geführt wird. Die seltene, aber
gravierende Konstellation gehört in einen eigenen Speicher, statt einen Massenspeicher
hochzuhalten.

## BSI-Vektoren geprüft 2026-08-10

**Vertraulichkeit sehr hoch, Integrität hoch, Verfügbarkeit normal.**

Die Vertraulichkeit folgt hier ausnahmsweise nicht nur der Datenschutzstufe, sondern auch dem
Institutionsschaden: Ein Verstoß gegen § 13 SBGG ist bußgeldbewehrt und träfe die Kommune als
Verantwortliche unmittelbar.

Die Integrität ist hoch, weil eine falsche Zuordnung von altem und neuem Namen dieselbe Wirkung
hätte wie eine Offenbarung -- sie brächte einen Menschen mit einer Identität in Verbindung, die
nicht seine ist. Die Verfügbarkeit bleibt normal: An diesen Bestand knüpft keine Frist, und im
Zweifel ist Nichtverfügbarkeit hier die sichere Richtung.
