---
id: dstore-schwerbehinderung-beschaeftigte
bereich: intern
typ: datenspeicher
system: null
name: Schwerbehinderung der Beschäftigten
zuständige-einheit: oe-amt-11
personenbezug: ja
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. b
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  - gesetz: NBG
    artikel: § 88 Abs. 1, § 94 Abs. 1
  - gesetz: SGB IX
    artikel: § 2 Abs. 3, § 163, § 178, § 208
  aufbewahrung:
    frist: 5 Jahre
    beginn: nach Abschluss der Personalakte
    hinweis: 'Frist der Personalakte nach § 94 Abs. 1 NBG; gilt nach § 12 Abs. 1 NDSG auch für Tarifbeschäftigte.'
letzte-aktualisierung: '2026-10-05'
tags:
- Personal
- Schwerbehinderung
- Gesundheitsdaten
- Beschäftigtendaten
---

# Schwerbehinderung der Beschäftigten

## Definition

Anerkannte Schwerbehinderung oder Gleichstellung von Beschäftigten der Kommune, soweit die Personalstelle sie für Zusatzurlaub, Beteiligung der Schwerbehindertenvertretung und die Anzeige zur Beschäftigungsquote benötigt.

## Felder

- Name und Personalnummer
- Grad der Behinderung
- Merkzeichen
- Gültigkeit des Nachweises
- Gleichstellung nach § 2 Abs. 3 SGB IX
- daraus folgende Ansprüche (Zusatzurlaub, Arbeitsplatzausstattung)
- Datum der Vorlage
- Beteiligung der Schwerbehindertenvertretung

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). Die Angabe lief bis dahin über `dstore-schwerbehindertennachweis`, der am 05.10.2026 auf extern gesetzt wurde (16 externe gegen 5 interne Verwendungen).

**Bewerbende nicht hier.** Nach D1 werden Angaben Bewerbender im Bewerberspeicher `dstore-bewerbungsunterlagen` geführt (Frist 6 Monate nach Absage) und erst bei Einstellung hierher übernommen.

**Schutzstufe D.** Gesundheitsdatum nach Art. 9 Abs. 1 DSGVO.

**BSI-Vektoren.** Vertraulichkeit hoch. Integrität normal: Der Nachweis kann erneut vorgelegt werden. Verfügbarkeit normal.

**Abgrenzung:**
- `dstore-schwerbehindertennachweis`: Nachweis in Bürgerverfahren (Parkausweise, Eingliederungshilfe), extern.
- `dstore-urlaubs-und-abwesenheitsdaten`: genommener Urlaub; der Anspruch auf Zusatzurlaub folgt aus diesem Speicher.
