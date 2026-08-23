---
id: dstore-todesbescheinigung
typ: datenspeicher
system: null
name: Todesbescheinigung
zuständige-einheit: oe-amt-53
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
  - gesetz: Nds. BestattG
    artikel: § 6 Abs. 3
  - gesetz: Nds. BestattG
    artikel: § 6 Abs. 4
  aufbewahrung:
    frist: 30 Jahre
    beginn: nach dem Sterbedatum
    hinweis: § 6 Abs. 5 Nds. BestattG.
letzte-aktualisierung: '2026-08-10'
tags:
- Bestattungswesen
- Todesbescheinigung
---



# Todesbescheinigung

## Definition

Bescheinigung über den Tod einer Person einschließlich der Todesursache nach § 6 Abs. 3 Nds. BestattG sowie die Vermerke über gewährte Einsichtnahmen.

## Felder

- Verstorbene Person
- Sterbedatum und Sterbeort
- Todesursache (vertraulicher Teil)
- feststellende Ärztin oder Arzt
- Einsichtnahmen mit Datum, einsehender Person und nachgewiesenem Interesse

## Hinweise

Angelegt am 2026-08-03 zu `vvt-53-004` (Einsichtnahme in Todesbescheinigungen).

**Die verstorbene Person ist nicht Betroffene der DSGVO** -- der Schutz der Verordnung endet mit dem Tod. Die Todesursache lässt aber Rückschlüsse auf lebende Angehörige zu, etwa bei Erbkrankheiten. Das trägt die Einstufung in Stufe D unabhängig davon, dass Art. 9 DSGVO auf die verstorbene Person nicht anwendbar ist.

Der vertrauliche Teil der Todesbescheinigung ist vom nichtvertraulichen getrennt zu halten; das Einsichtsrecht nach § 6 Abs. 4 Nds. BestattG reicht nicht auf beide Teile gleich weit.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Der Bestand ist Grundlage einer Entscheidung über einen Menschen. Eine unbemerkte Verfälschung führt zu einer falschen Entscheidung, die für die betroffene Person unmittelbare Folgen hat und im Nachhinein kaum aufzuklären ist.

Sie ist Grundlage für Bestattung, Sterbeurkunde und Erbfolge und enthält die Todesursache.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Gesundheit und andere besondere Kategorien nach Art. 9 DSGVO.** Die Verarbeitung ist grundsätzlich untersagt und nur zulässig, wenn ein Ausnahmetatbestand des Art. 9 Abs. 2 DSGVO greift. Das LfD-Schutzstufenkonzept ordnet diese Angaben der Stufe D zu; die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Praktische Folge:** Für diese Speicher ist der Zugriff auf die Personen zu beschränken, die ihn zur Aufgabenerfüllung brauchen -- eine amtsärztliche Stellungnahme gehört nicht in die allgemeine Personalakte, sondern in einen gesondert geführten Teilbestand.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
