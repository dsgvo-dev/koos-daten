---
id: dstore-mitgliedschaft-realverband
typ: datenspeicher
system: null
name: Mitgliedschaft und Beiträge Realverband
zuständige-einheit: oe-amt-86
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. b, lit. c und lit. e
  - gesetz: Nds. RealVerbG
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Ende der Mitgliedschaft
letzte-aktualisierung: '2026-08-10'
tags:
- Realverband
- Wegegenossenschaft
- Mitgliedschaft
---


# Mitgliedschaft und Beiträge Realverband

## Definition

Mitgliedschafts- und Beitragsdaten in Realverbänden und Wegegenossenschaften, deren Aufsicht der Kommune obliegt.

## Felder

- Mitglied (natürliche oder juristische Person)
- zugrunde liegendes Flurstück
- Anteil oder Stimmrecht
- Beitragspflicht und Beitragshöhe
- Zahlungsstand
- Beginn und Ende der Mitgliedschaft

## Hinweise

Angelegt am 2026-08-03 zu `vvt-86-002` (Verwaltung von Wegegenossenschaften und Realverbänden).

**Kein kommunaler Gebührentatbestand.** Beiträge eines Realverbands beruhen auf dessen Satzung, nicht auf dem NKAG. `dstore-gebuehrenbescheid-zahlungsdaten` passt deshalb nicht.

Die Mitgliedschaft folgt dem Grundstückseigentum; sie wechselt mit dem Eigentum, ohne dass die betroffene Person darauf Einfluss hat.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Die Mitgliedschaft folgt dem Grundstückseigentum und begründet Beitragspflichten. Ein falscher Bestand belastet die falsche Person.

## Schutzstufe geprüft 2026-08-10

**B → C.** Das Feld **Zahlungsstand** trägt die Anhebung. Ein Beitragsrückstand im Realverband wird nach § 26 RealVerbG im Verwaltungszwangsverfahren beigetrieben; die Angabe ist damit ein Hinweis auf Zahlungsschwierigkeiten. Anteil und Stimmrecht lassen zudem die Größe des Grundbesitzes erkennen.

Stufe D wäre erreicht, sobald Vollstreckungsmaßnahmen dokumentiert werden -- die gehören in `dstore-vollstreckungsdaten`.
