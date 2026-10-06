---
id: dstore-fuehrungszeugnis-bewerbende
bereich: intern
typ: datenspeicher
system: null
name: Führungszeugnis der Bewerbenden
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
    artikel: Art. 10
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  - gesetz: NBG
    artikel: § 88 Abs. 1
  - gesetz: BZRG
    artikel: § 30
  - gesetz: SGB VIII
    artikel: § 72a (bei Tätigkeiten mit Kindern und Jugendlichen)
  aufbewahrung:
    frist: 6 Monate
    beginn: nach Abschluss des Bewerbungsverfahrens (Absage)
    hinweis: 'Frist wie Bewerbungsunterlagen (§ 15 Abs. 4 AGG). Bei Einstellung wird der Einsichtnahmevermerk in die Personalakte übernommen (§ 94 Abs. 1 NBG).'
letzte-aktualisierung: '2026-10-05'
tags:
- Personal
- Bewerbung
- Führungszeugnis
- Art. 10 DSGVO
---

# Führungszeugnis der Bewerbenden

## Definition

Vermerk über die Einsichtnahme in ein Führungszeugnis, das Bewerbende für eine Stelle vorlegen, für die es erforderlich ist (etwa Kassenbefugnis oder Tätigkeit mit Kindern und Jugendlichen). Das Führungszeugnis selbst wird eingesehen und zurückgegeben; aufbewahrt wird nur der Vermerk (Entscheidung Martin 05.10.2026, Option A).

## Felder

- Name der bewerbenden Person
- Stelle
- Grund der Anforderung (Rechtsgrundlage für die Stelle)
- Datum des Führungszeugnisses
- Datum der Einsichtnahme
- Ergebnis: Einträge ja/nein; Erheblichkeit für die Stelle
- einsehende Person

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). Das Führungszeugnis der Bewerbenden lief bis dahin über `dstore-fuehrungszeugnis`. Dieser Speicher wurde am 05.10.2026 auf extern gesetzt, weil er überwiegend von Bürgerverfahren genutzt wird (20 externe gegen 2 interne Verwendungen).

**Nur Vermerk, keine Kopie.** Der Vermerk genügt für die Auswahlentscheidung und hält die Menge der Daten über Straftaten gering (Art. 5 Abs. 1 lit. c DSGVO). § 72a Abs. 5 SGB VIII schreibt dieses Vorgehen für Tätigkeiten mit Kindern und Jugendlichen ausdrücklich vor.

**Schutzstufe D.** Daten über Straftaten nach Art. 10 DSGVO; Stufe wie `dstore-fuehrungszeugnis`.

**BSI-Vektoren.** Vertraulichkeit hoch: Bekanntwerden belastet die Person erheblich. Integrität normal: Das Zeugnis kann erneut beantragt werden. Verfügbarkeit normal.

**Abgrenzung:**
- `dstore-fuehrungszeugnis`: Führungszeugnisse in Bürgerverfahren (Gewerbe, Waffen, Pflegeeltern u. a.), extern.
- `dstore-sicherheitserkenntnisse`: Erkenntnisse der Sicherheitsüberprüfung (10-029), nicht das Führungszeugnis.
- `dstore-bewerbungsunterlagen`: übrige Bewerbungsunterlagen; das Führungszeugnis ist wegen Art. 10 DSGVO getrennt geführt.
