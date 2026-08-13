---
id: dstore-antragsbegruendung-schulbezirk
typ: datenspeicher
system: null
name: Begründung eines Ausnahmeantrags zum Schulbesuch
datenkategorie: Bildung & Schule
zuständige-einheit: oe-amt-40
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
    artikel: Art. 9 Abs. 2 lit. g
  - gesetz: NDSG
    artikel: § 17
  - gesetz: NSchG
    artikel: § 63 Abs. 3
  aufbewahrung:
    frist: bis zum Ende des Schulbesuchs an der aufnehmenden Schule
    beginn: mit Bestandskraft der Entscheidung
    hinweis: Die Begründung wird nur solange benötigt, wie die Ausnahme trägt. Sie
      ist getrennt von der Schülerakte zu führen.
letzte-aktualisierung: '2026-08-10'
tags:
- Schule
- Art. 9 DSGVO
- Schulbezirk
---


# Begründung eines Ausnahmeantrags zum Schulbesuch

## Definition

Von den Erziehungsberechtigten vorgetragene Gründe für eine Ausnahme vom Schulbezirk, soweit sie familiäre Notlagen, Behinderungen oder Gesundheitszustände betreffen.

## Felder

- Antragstellende Person
- betroffenes Kind
- vorgetragener Grund
- beigefügte Nachweise
- Stellungnahme der abgebenden und der aufnehmenden Schule
- Entscheidung und Datum

## Hinweise

Angelegt am 2026-08-03 zu `vvt-40-010` (Ausnahmeanträge zum Schulbesuch), nach Auskunft des Fachamts vom 2026-08-03.

**Stufe D, weil die Begründung regelmäßig besondere Kategorien enthält.** Ausnahmen vom Schulbezirk werden mit Gesundheitszuständen, Behinderungen oder familiären Notlagen begründet -- Angaben nach Art. 9 Abs. 1 DSGVO.

**Getrennt von der übrigen Schulverwaltung zu führen.** Die Gründe sind für die Entscheidung erforderlich, nicht für den laufenden Schulbetrieb. Wer die Ausnahme kennt, muss die Begründung nicht kennen.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Familiäre, aufenthaltsrechtliche und weltanschauliche Verhältnisse.** Anders als bei den am selben Tag herabgestuften Personenstandsspeichern trägt dieser Bestand eine Angabe, die für sich genommen belastend ist -- eine Sorgerechtsentscheidung, die Abstammung, die Religionszugehörigkeit, den Aufenthaltsstatus oder die Ausübung eines Grundrechts. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
