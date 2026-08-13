---
id: dstore-nachlass-erbendaten
typ: datenspeicher
system: null
name: Nachlass- und Erbendaten
datenkategorie: Finanzen & Vollstreckung
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: SGB XII
    artikel: § 102
  - gesetz: SGB XII
    artikel: §§ 93, 94
  - gesetz: BGB
    artikel: §§ 1922 ff.
  aufbewahrung:
    frist: 6 Jahre
    beginn: nach Abschluss des Rückforderungsverfahrens
    hinweis: § 102 Abs. 4 SGB XII (Erlöschen des Kostenersatzanspruchs drei Jahre
      nach dem Tod), zuzüglich Vollstreckungszeitraum.
letzte-aktualisierung: '2026-08-10'
tags:
- Sozialhilfe
- Nachlass
- Kostenersatz
---



# Nachlass- und Erbendaten

## Definition

Angaben über Nachlass, Erben, Beschenkte und Pflichtteilsberechtigte, soweit sie für die Überleitung von Ansprüchen und den Kostenersatz nach dem SGB XII erforderlich sind.

## Felder

- Erblasser oder Erblasserin
- Erben, Beschenkte, Pflichtteilsberechtigte
- Verwandtschaftsverhältnis
- Nachlassgegenstände einschließlich Grundbesitz
- Wert des Nachlasses
- Erbschein oder Testament
- Stand der Überleitung

## Hinweise

Angelegt am 2026-08-03 zu `vvt-50-002` (Rückforderung von Sozialhilfe und Überleitung von Ansprüchen).

Die VVT führte „Nachlassdaten" als Datenart und das Katasteramt als Empfänger, ohne dass ein Speicher dafür bestand. Betroffene sind ausdrücklich auch Personen, die selbst nie Leistungen bezogen haben -- Erben, Beschenkte, Pflichtteilsberechtigte. Sie erfahren von der Verarbeitung regelmäßig erst durch die Inanspruchnahme; die Informationspflicht nach Art. 14 DSGVO ist dabei zu beachten.

## Einstufung nach dem Maximalprinzip 2026-08-03

Die Schutzstufe richtet sich nach der sensibelsten Angabe, die in diesem Speicher anfallen **kann** -- nicht nach dem Regelfall. Ist die Verarbeitung von Daten nach Art. 9 Abs. 1 DSGVO möglich, gilt für den Speicher insgesamt die höhere Stufe.

Der Grund ist praktischer Natur: Technische und organisatorische Maßnahmen werden für den Speicher eingerichtet, nicht für den einzelnen Datensatz. Eine Einstufung, die erst im Einzelfall angehoben wird, führt zu Maßnahmen, die im Einzelfall nicht greifen.

**Von C auf D.** Der Speicher entsteht im Verfahren der Rückforderung von Sozialhilfe. Schon die Existenz eines Eintrags offenbart, dass die verstorbene Person Leistungen nach dem SGB XII bezogen hat -- ein Sozialdatum, das das LfD-Konzept ausdrücklich der Stufe D zuordnet. Betroffen sind zudem Erben und Beschenkte, die selbst nie Leistungen bezogen haben und von der Verarbeitung erst durch die Inanspruchnahme erfahren.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `hoch`** · **Verfügbarkeit: `hoch`**

**Über `normal` gesetzt: Integrität `hoch` und Verfügbarkeit `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** Die Einstufung wurde am 2026-08-04 bei der Anlage beziehungsweise
Überarbeitung dieses Speichers ausführlich begründet -- siehe die Hinweise oben. Der
Durchgang vom 2026-08-10 hat sie bestätigt und trägt hier nur den Prüfvermerk nach, der bisher
fehlte.

*Der Vermerk ist kein Formalismus: Ohne ihn zählte der Speicher als ungeprüft, und der
Rückstand wies 129 statt der tatsächlich offenen 115 Speicher aus -- allesamt auf Stufe C.*
