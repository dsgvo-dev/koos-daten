---
id: dstore-bewerbungsunterlagen
bereich: intern
typ: datenspeicher
system: null
name: Bewerbungsunterlagen
zuständige-einheit: oe-amt-11
bpmn:
  typ: datenspeicher
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
  - gesetz: AGG
  - gesetz: DSGVO
  aufbewahrung:
    frist: 6 Monate nach Absage
    beginn: prozessabhängig
letzte-aktualisierung: '2026-10-05'
tags:
- Bewerbung
- Stellenausschreibung
- HR
konvertiert-aus: daten1/dtype-bewerbungsunterlagen.md
---


## Beschreibung

Unterlagen einer Stellenbewerbung: Lebenslauf, Zeugnisse, Anschreiben.

## Felder

- Bewerber
- Stelle
- Lebenslauf
- Zeugnisse
- Anschreiben
- Eingangsdatum
- Name, Vorname, Geburtsdatum und -ort, Anschrift, Kontaktdaten (Stammdaten der Bewerbenden, D1)
- Staatsangehörigkeit, soweit für das Beamtenverhältnis erheblich (§ 7 BeamtStG)
- Schwerbehinderung oder Gleichstellung, soweit zur bevorzugten Berücksichtigung angegeben (§ 165 SGB IX)

## Rechtsgrundlage

AGG, DSGVO

## Löschfrist

6 Monate nach Absage

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Beschäftigtendaten mit Bewertungsbezug.** Das LfD-Schutzstufenkonzept nennt dienstliche Beurteilungen ausdrücklich bei Stufe D. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Hinzu kommt das Abhängigkeitsverhältnis:** Beschäftigte können der Verarbeitung nicht ausweichen, und eine Offenlegung innerhalb der Verwaltung wirkt im täglichen Zusammenarbeiten fort. Für die Personalakte gilt zudem § 88 NBG mit einem eigenen Zugriffsregime, das strenger ist als das allgemeine Datenschutzrecht.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*

## Erweitert 2026-10-05 (D1, Bewerberspeicher)

Nach Entscheidung D1 (Martin, 05.10.2026) ist dieser Speicher der Bewerberspeicher: Er nimmt die Stammdaten der Bewerbenden, die Staatsangehörigkeit und die Angabe zur Schwerbehinderung auf, die vorher in den externen Speichern `dstore-personenstammdaten-vertraulich`, `dstore-staatsangehoerigkeit` und `dstore-schwerbehindertennachweis` geführt wurden. Frist bleibt 6 Monate nach Absage. Bei Einstellung werden die übernommenen Daten in `dstore-personalstammdaten-beschaeftigte` und `dstore-schwerbehinderung-beschaeftigte` überführt. Das Führungszeugnis wird wegen Art. 10 DSGVO getrennt in `dstore-fuehrungszeugnis-bewerbende` vermerkt.
