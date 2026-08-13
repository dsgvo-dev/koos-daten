---
id: dstore-baugenehmigung
typ: datenspeicher
system: null
name: Baugenehmigung
datenkategorie: Bescheid / Nachweis
zuständige-einheit: oe-amt-63
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
  - gesetz: NBauO
    artikel: §70
    titel: Baugenehmigung
  - gesetz: VwVfG
    artikel: §37
    titel: Bestimmtheit von Verwaltungsakten
  - gesetz: NBauO
    artikel: §79
    titel: Geltungsdauer
  aufbewahrung:
    frist: dauerhaft
    beginn: null
    hinweis: Dauerhafter Bestandteil der Bauakte; Genehmigung bleibt rechtlich relevant
letzte-aktualisierung: '2026-08-10'
---


# Baugenehmigung

## Definition

Verwaltungsakt der Bauaufsichtsbehörde, mit dem ein Bauvorhaben nach Prüfung der
öffentlich-rechtlichen Vorschriften genehmigt wird. Die Baugenehmigung ist Voraussetzung
für den Baubeginn (§ 70 NBauO).

## Typische Inhalte

- Bezeichnung des genehmigten Vorhabens und Grundstücks
- Auflagen und Bedingungen (z.B. Brandschutzauflagen)
- Gültigkeitsdauer (i.d.R. 3 Jahre; § 79 NBauO)
- Stempel und Unterschrift der Bauaufsichtsbehörde
- Stempel auf den genehmigten Bauzeichnungen

## Hinweise

Die Baugenehmigung erlischt, wenn mit dem Bau nicht innerhalb der Geltungsdauer begonnen
wird oder das Vorhaben für mehr als ein Jahr unterbrochen wird (§ 79 NBauO).
Verlängerung ist auf Antrag möglich (proc-verlaengerung-der-geltungsdauer-von-baugenehmigung).

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Sie begründet Bestandsschutz und wird noch nach Jahrzehnten herangezogen.

## Schutzstufe geprüft 2026-08-10

**B → C.** Die Bau-Grunddaten sind mehr als Sachdaten.

Der Bescheid enthält Auflagen und, bei einer Abweichung nach § 66 NBauO, die Begründung des Einzelfalls. Ablehnungen und Rücknahmen dokumentieren ein Scheitern, das mit erheblichen Kosten verbunden ist.

**Kohärenz:** `dstore-bauakte` steht seit dem 2026-08-10 auf Stufe D, weil sie die Nachbareinwendung aufnimmt. Die Einzelbestandteile tragen diese Stufe nicht -- sie tragen aber auch nicht mehr die Stufe B, die sie aus dem Import mitgebracht hatten.
