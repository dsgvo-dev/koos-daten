---
id: dstore-verwahrgut-sicherstellung
typ: datenspeicher
system: null
name: Verwahrgut aus Sicherstellung
datenkategorie: Sicherheit & Ordnung
zuständige-einheit: oe-amt-20
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
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: NDSG
    artikel: § 3
  - gesetz: NPOG
    artikel: §§ 26 bis 29
  aufbewahrung:
    frist: 3 Jahre
    beginn: nach Rückgabe an die berechtigte Person oder nach Verwertung
    hinweis: Festlegung des Trägers, angelehnt an die regelmäßige Verjährung des Kostenerstattungsanspruchs
      nach § 29 NPOG. Ist ein Streit über Herausgabe oder Kosten anhängig, wird bis
      zum rechtskräftigen Abschluss aufbewahrt.
letzte-aktualisierung: '2026-08-04'
tags:
- Sicherstellung
- Verwahrung
- Ordnungsrecht
---



# Verwahrgut aus Sicherstellung

## Definition

Nachweis über Gegenstände, die nach § 26 NPOG sichergestellt und nach § 27 NPOG in Verwahrung genommen wurden, bis zu ihrer Herausgabe nach § 29 NPOG oder ihrer Verwertung nach § 28 NPOG.

## Felder

- laufende Nummer des Verwahrvorgangs
- Grund und Zeitpunkt der Sicherstellung, anordnende Stelle
- Person, gegenüber der sichergestellt wurde
- berechtigte Person, soweit sie von dieser abweicht
- Beschreibung und geschätzter Wert des Gegenstands
- Verwahrort
- Herausgabevermerk mit Datum und empfangender Person
- Verwertungs- oder Vernichtungsvermerk mit Erlös
- Kostenforderung nach § 29 NPOG und deren Erledigung

## Hinweise

Angelegt am 2026-07-30 zusammen mit `proc-sichergestellte-gegenstaende-verwahren-und-herausgeben` und `vvt-20-003`. Für Sicherstellung und Verwahrung war im Bestand kein Speicher vorhanden.

**Die berechtigte Person ist ein eigenes Feld.** § 29 NPOG verlangt die Herausgabe an die berechtigte Person -- das ist nicht zwingend die Person, bei der sichergestellt wurde. Ohne getrenntes Feld lässt sich die Herausgabepflicht nicht erfüllen und die Rechtmäßigkeit der Herausgabe nicht belegen.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Der Bestand begründet den Herausgabeanspruch nach § 29 NPOG. Ohne verlässlichen Nachweis ist nicht feststellbar, wem was gehört.

## Schutzstufe geprüft 2026-08-13

**C bestätigt.** Sicherstellung nach §§ 26–29 NPOG ist eine eingreifende ordnungsrechtliche
Maßnahme — C. Die effektive Stufe D entsteht in vvt-20-003 über den Kontext
(`personenstammdaten-vertraulich` D, ADR 010), nicht über diesen Speicher.

Geprüft im Rahmen der Schutzstufendurchsicht Los 3 (Amt 20). Vorschlag:
`_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-13-los3-amt20-korrigiert.md`.
