---
id: dstore-hebammenanzeige
typ: datenspeicher
system: null
name: Anzeige und Aufsicht Hebammen
zuständige-einheit: oe-amt-53
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: Nds. HebG
    artikel: § 7
  - gesetz: Nds. HebG
    artikel: § 8
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Beendigung der Tätigkeit im Zuständigkeitsbereich
letzte-aktualisierung: '2026-08-04'
tags:
- Hebammen
- Berufsaufsicht
---



# Anzeige und Aufsicht Hebammen

## Definition

Angaben zur Anzeige der Berufsausübung und zur Aufsicht über Hebammen nach dem Niedersächsischen Hebammengesetz.

## Felder

- Hebamme
- Berufsbezeichnung und Erlaubnis
- Anzeige der Tätigkeitsaufnahme mit Datum
- Tätigkeitsort
- Fortbildungsnachweis
- Aufsichtsvorgänge und Beanstandungen

## Hinweise

Angelegt am 2026-08-03 zu `vvt-53-003` (Berufsaufsicht Heilberufe).

Die VVT bündelt Hebammen und Heilpraktiker. Für die Heilpraktikerseite bestand `dstore-heilpraktikererlaubnisverfahren`, für die Hebammenseite nichts. Die Anzeige nach § 7 Nds. HebG und die Aufsicht nach § 8 sind ein eigenes Verfahren mit eigener Rechtsgrundlage.

## Schutzstufe geprüft 2026-08-14

**C bestätigt.** Berufsdaten einer Hebamme (Erlaubnis, Tätigkeitsort, Fortbildung) und Aufsichtsvorgänge nach § 7/8 Nds. HebG. Berufsaufsichtliche Beanstandungen sind berufsrechtlich relevant, aber keine Art. 9-Daten. C ist angemessen.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.
