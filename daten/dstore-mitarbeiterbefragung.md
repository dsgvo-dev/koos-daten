---
id: dstore-mitarbeiterbefragung
typ: datenspeicher
system: null
name: Mitarbeiterbefragung
zuständige-einheit: oe-amt-11
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
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 88 (Beschäftigtendatenschutz)
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. b (bei Fragen zum Gesundheitszustand)
  - gesetz: NDSG
    artikel: § 12
  - gesetz: ArbSchG
    artikel: § 5 Abs. 3 Nr. 6 (Gefährdungsbeurteilung psychischer Belastung)
  aufbewahrung:
    frist: Rohdaten unverzüglich nach Abschluss der Auswertung
    beginn: Auswertungsabschluss
    hinweis: Anonymisierte Ergebnisse und Auswertungsbericht nach Dienstvereinbarung,
      in der Regel 3-10 Jahre. Bei externem Institut Löschung der Rohdaten nach
      Art. 28 Abs. 3 lit. g DSGVO.
letzte-aktualisierung: '2026-08-29'
tags:
- Befragung
- Beschäftigtendatenschutz
- Psychische Belastung
---


# Mitarbeiterbefragung

## Definition

Antworten und Rohdaten aus Befragungen der Beschäftigten — zur Arbeitszufriedenheit, zu
psychischen Belastungen oder zu organisatorischen Themen. Der Speicher umfasst den Bestand
bis zur Löschung der Rohdaten; der anonymisierte Auswertungsbericht ist kein
personenbezogener Datenbestand und wird hier nicht geführt.

## Felder

- Antworten (strukturiert)
- Antworten (Freitext)
- Demografische Angaben (Altersgruppe, Geschlecht, Organisationseinheit, Dauer der Betriebszugehörigkeit)
- Pseudonyme Teilnahmekennung
- Rohdatensatz bis zur Löschung

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenobjekt

## Schutzstufe geprüft 2026-08-29

**D bei Anlage.** Freie Antwortfelder und Fragen zu psychischen Belastungen lassen Daten
nach Art. 9 DSGVO zu; die Rechtsgrundlage der Verarbeitung `vvt-11-015` nennt Art. 9
ausdrücklich, der Zweck nennt § 5 Abs. 3 Nr. 6 ArbSchG. Das LfD-Schutzstufenkonzept ordnet
Angaben nach Art. 9 der Stufe D zu.

**Die Pseudonymisierung senkt die Stufe nicht.** Die pseudonyme Teilnahmekennung ist eine
technische Maßnahme, keine Herabstufung — `reg-klassifizierung` 3.5.4. Der anonymisierte
Auswertungsbericht ist davon zu trennen: er ist nach derselben Ziffer als Stufe A zu führen
und wird nicht als Datenspeicher geführt.

**Weg zu einer Herabstufung.** Ergibt der freigegebene Fragebogen, dass weder nach dem
Gesundheitszustand gefragt wird noch Freitextfelder vorgesehen sind, ist C nach 4.3
möglich — mit Begründung und Bestätigung durch die zuständige Fachbereichsleitung,
festgehalten in der Dienstvereinbarung. Nach 4.3 ist im Zweifel die höhere Stufe zu wählen;
die Herabstufung ist der vorgesehene Weg, nicht die nachträgliche Anhebung.

## BSI-Vektoren geprüft 2026-08-29

**Vertraulichkeit hoch.** Ein Bekanntwerden einzelner Antworten beschädigt das Vertrauen in
das Befragungsverfahren und damit dessen Zweck; ohne zugesicherte Vertraulichkeit ist eine
Beteiligung nicht zu erwarten.

**Integrität normal.** Die Rohdaten sind eine Momentaufnahme freiwilliger Angaben, kein
Bestand, auf dessen Richtigkeit sich Dritte verlassen. Eine Verfälschung verzerrt die
Auswertung, begründet aber keine Rechtsfolge.

**Verfügbarkeit normal.** Die Rohdaten werden nach der Auswertung gelöscht; ein Ausfall
verzögert die Auswertung, ohne eine Aufgabe zu blockieren.

## Rechtsgrundlagen

- DSGVO Art. 88 i. V. m. NDSG § 12 (Beschäftigtendatenschutz)
- DSGVO Art. 9 Abs. 2 lit. b (bei Fragen zum Gesundheitszustand)
- ArbSchG § 5 Abs. 3 Nr. 6 (Gefährdungsbeurteilung psychischer Belastung)

## Hinweise

Die Auswertung erfolgt erst ab einer Mindestbesetzung je Auswertungseinheit (fünf bis zehn
Antworten, festgelegt in der Dienstvereinbarung). Kleinstauswertungseinheiten und
Filterführungen über offene Fragen können sonst eine Personenbeziehbarkeit herstellen,
auch wenn das Ziel die aggregierte Auswertung ist.
