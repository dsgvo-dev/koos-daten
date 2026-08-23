---
id: dstore-vorsorge-betreuungsvollmacht
typ: datenspeicher
system: null
name: Vorsorge- und Betreuungsvollmacht
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
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: BGB
    artikel: §§ 1814 ff. (Betreuungsrecht, Vorsorgevollmacht)
  - gesetz: SGB XII
    artikel: (Sozialhilfe, soweit einschlägig)
  - gesetz: Nds. AGBtG
    artikel: (Ausführung des Betreuungsrechts)
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Abschluss des Verfahrens
    hinweis: Fachlich zu validieren. Vorsorgevollmachten bleiben bis zum Widerruf wirksam;
      Bestellungen nach dem Betreuungsrecht bis zur Aufhebung durch das Gericht.
letzte-aktualisierung: '2026-08-14'
tags:
- Vorsorgevollmacht
- Betreuungsvollmacht
- Betreuung
- Sozialbereich
---

# Vorsorge- und Betreuungsvollmacht

## Definition

Vorsorge- und Betreuungsvollmachten, die im Sozialbereich — insbesondere bei der
Betreuungsbehörde und im Sozialamt — vorgelegt oder verarbeitet werden. Die Datenart belegt,
dass eine Person für den Fall der eigenen Handlungsunfähigkeit eine andere Person
bevollmächtigt hat oder unter rechtlicher Betreuung steht.

## Felder

- Vollmachtgeber beziehungsweise betreute Person
- Bevollmächtigte beziehungsweise Betreuerin oder Betreuer
- Umfang der Vollmacht (Aufgabenkreise)
- Bestellungsbeschluss des Betreuungsgerichts
- Datum und Unterschrift

## Hinweise

Angelegt am 2026-08-14 im Rahmen der Schutzstufendurchsicht Los 4 (Amt 10). Ersetzt den
bisherigen `dstore-vollmacht` (0 Verwendungen, „Vollmacht zur Vertretung").

**Abgrenzung:** Die „normale" Vollmacht zur Vertretung im Verwaltungsverfahren ist kein
eigenständiger Speicher — sie ist ein Schriftstück in der Verwaltungsakte und wird über
`dstore-verwaltungsakte` geführt. Dieser Speicher führt allein die Vorsorge- und
Betreuungsvollmacht im Sozialbereich.

**Die bloße Existenz offenbart:** Dass die Person für den Fall der Handlungsunfähigkeit
vorgesorgt hat oder unter rechtlicher Betreuung steht — eine Angabe über die rechtliche
Handlungsfähigkeit und damit über den Gesundheitszustand. Das trägt Stufe D.

## BSI-Vektoren geprüft 2026-08-14

**Vertraulichkeit: `hoch`** · **Integrität: `hoch`** · **Verfügbarkeit: `normal`**

- **Vertraulichkeit `hoch`:** Trägt denselben Befund wie die Datenschutz-Schutzstufe D —
  ein Datenschutzverstoß (Offenbarung einer rechtlichen Betreuung) ist für die Kommune
  Bußgeld- und Reputationsrisiko.
- **Integrität `hoch`:** Eine verfälschte oder gefälschte Vorsorge-/Betreuungsvollmacht
  ermöglicht Handlungen gegen den Willen der betroffenen Person. Der Bestand ist
  Entscheidungsgrundlage darüber, wer für eine andere Person handeln darf.
- **Verfügbarkeit `normal`:** Knüpft keine Frist oder Gefahrenlage an die sofortige
  Abrufbarkeit; ein Ausfall verzögert die Bearbeitung, ohne eine Frist verfallen zu lassen.

## Schutzstufe geprüft 2026-08-14

**D.** Die Vorsorge- oder Betreuungsvollmacht im Sozialbereich offenbart, dass eine Person
für den Fall der eigenen Handlungsunfähigkeit vorgesorgt hat oder unter rechtlicher
Betreuung steht. Das berührt den höchstpersönlichen Bereich und kann Gesundheitsdaten
(Art. 9 DSGVO) sowie Sozialdaten (§ 67 SGB X) offenbaren — das LfD-Konzept ordnet beides
der Stufe D zu.

Geprüft im Rahmen der Schutzstufendurchsicht Los 4 (Amt 10). Vorschlag:
`_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-14-los4-amt10.md`.
