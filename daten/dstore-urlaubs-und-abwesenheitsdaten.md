---
id: dstore-urlaubs-und-abwesenheitsdaten
typ: datenspeicher
system: null
name: Urlaubs- und Abwesenheitsdaten
zuständige-einheit: oe-amt-11
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
    artikel: Art. 6 Abs. 1 lit. b und lit. c
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. b
  - gesetz: NDSG
    artikel: § 12
  - gesetz: NBG
    artikel: §§ 88, 94
  - gesetz: BUrlG
  - gesetz: TVöD
  aufbewahrung:
    frist: 3 Jahre
    beginn: nach Ablauf des Jahres, in dem die Bearbeitung des einzelnen Urlaubsvorgangs
      abgeschlossen wurde
    hinweis: Frist aus § 94 Abs. 2 Satz 1 NBG für Unterlagen über Erholungsurlaub.
      Soweit Urlaubsunterlagen in die Personalakte übernommen werden, gilt für diese
      § 94 Abs. 1 NBG mit fünf Jahren nach Abschluss der Personalakte.
letzte-aktualisierung: '2026-08-04'
tags:
- Personal
- Urlaub
- Abwesenheit
- Beschäftigtendaten
---


# Urlaubs- und Abwesenheitsdaten

## Definition

Daten zur Planung, Bewilligung und Abrechnung von Urlaub und sonstigen Abwesenheiten der Beschäftigten, geführt im Zeitwirtschafts- oder Personalmanagementsystem.

## Felder

- Personalnummer und Name
- Organisationseinheit
- Urlaubsanspruch des Jahres, Resturlaub und Übertrag
- verplante und tatsächlich genommene Urlaubstage
- Zeitraum der Abwesenheit
- Urlaubsart (Erholungsurlaub, Sonderurlaub, Elternzeit, Bildungsurlaub, Zusatzurlaub nach § 208 SGB IX)
- Vertretungsregelung
- Status der Bewilligung und bewilligende Person

## Hinweise

Angelegt am 2026-07-30 zusammen mit `proc-urlaub-beantragen-und-bewilligen` und `vvt-11-003`. Urlaubsdaten waren im Bestand als Datenart benannt, aber ohne eigenen Datenspeicher geführt; die vorhandenen Personalspeicher treffen sie nicht, und für sie gilt mit drei Jahren eine kürzere Frist als für die Personalakte.

**Die Urlaubsart ist ein eigenes Feld mit eigener Sichtbarkeit.** Zusatzurlaub nach § 208 SGB IX offenbart eine Schwerbehinderung, Elternzeit und Sonderurlaub können Rückschlüsse auf familiäre oder gesundheitliche Umstände zulassen. Deshalb wird die Art getrennt von der allgemeinen Urlaubsübersicht geführt und erscheint nicht in Vertretungs- und Abwesenheitsplänen, die anderen Beschäftigten zugänglich sind. Dort steht ausschließlich die Abwesenheit als solche.

**Abgrenzung:** Die Aufzeichnung der täglichen Arbeitszeit — Kommt-, Geht- und Pausenzeiten, Zeitausgleich — gehört nicht hierher. Für sie gilt mit § 16 Abs. 2 ArbZG eine eigene Frist.

## Schutzstufe geprüft 2026-08-04

Durchsicht des Katalogs gegen das Schutzstufenkonzept des LfD Niedersachsen,
Maximalprinzip.

**Von C auf D -- wegen eines einzigen Feldwerts.** Das Feld „Urlaubsart" nennt ausdrücklich den **Zusatzurlaub nach § 208 SGB IX**. Dieser Anspruch steht ausschließlich schwerbehinderten Menschen zu. Wer ihn in Anspruch nimmt, ist damit in der Urlaubskartei als schwerbehindert erkennbar -- ein Datum nach Art. 9 Abs. 1 DSGVO.

Dasselbe gilt abgeschwächt für Elternzeit und Sonderurlaub aus familiären Anlässen. Die Urlaubsverwaltung wirkt harmlos und führt tatsächlich Angaben, für die anderswo eine eigene Rechtsgrundlage verlangt wird.

**Praktische Folge:** Die Urlaubsart sollte für die allgemeine Urlaubsplanung nicht sichtbar sein. Für die Vertretungsregelung genügt der Zeitraum.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*
