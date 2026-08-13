---
id: dstore-meldebescheinigung
name: Meldebescheinigung
datenkategorie: Bescheid / Nachweis
zuständige-einheit: oe-amt-33
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
  - gesetz: BMG
    artikel: §18
    titel: Meldebescheinigung
  aufbewahrung:
    frist: kein eigener Aufbewahrungsbedarf der Behörde
    beginn: null
    hinweis: Verbleibt bei der meldepflichtigen Person
letzte-aktualisierung: '2026-08-10'
---


# Meldebescheinigung

## Definition

Amtliche Bestätigung der Meldebehörde über die aktuelle Hauptwohnung einer Person.
Wird nach erfolgter Ummeldung auf Wunsch ausgestellt.

## Typische Inhalte

- Name, Geburtsdatum
- Aktuelle Hauptwohnung (Straße, PLZ, Ort)
- Datum der Ausstellung und Stempel der Meldebehörde

## Hinweise

Die einfache Meldebescheinigung ist in der Regel gebührenfrei.
Für beglaubigte Bescheinigungen oder Auszüge aus dem Melderegister können Gebühren
nach der Gebührensatzung der Gemeinde erhoben werden.
Meldebescheinigungen haben keine festgelegte Gültigkeitsdauer, werden aber von Behörden
oft nur als aktuell anerkannt, wenn sie nicht älter als 3 Monate sind.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Die Bescheinigung wird Dritten vorgelegt und genießt öffentlichen Glauben.

## Schutzstufe geprüft 2026-08-10

**B → C.** **Kohärenzkorrektur.** Die Bescheinigung enthält dieselbe Angabe wie `dstore-meldeadresse-wohnsitz` -- den Wohnort einer Person. Dass sie als Dokument und nicht als Registereintrag geführt wird, ändert an der Sensibilität nichts.

Die Anschrift ist die Angabe, an der die praktisch wichtigsten Schutzmaßnahmen des Melderechts hängen: die Auskunftssperre nach § 51 BMG bei Gefahr für Leben, Gesundheit oder Freiheit und der bedingte Sperrvermerk nach § 52 BMG. **Vor jeder Ausstellung ist zu prüfen, ob eine Sperre vorliegt** -- eine Meldebescheinigung, die an die falsche Person gerät, kann eine Schutzsuchende auffindbar machen.
