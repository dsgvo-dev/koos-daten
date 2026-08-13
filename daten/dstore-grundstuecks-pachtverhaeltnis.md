---
id: dstore-grundstuecks-pachtverhaeltnis
typ: datenspeicher
system: null
name: Grundstücks- und Pachtverhältnis
datenkategorie: Liegenschaften
zuständige-einheit: oe-amt-23
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: BGB
  - gesetz: NKomVG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Pacht
- Grundstück
- Vertrag
---


# Grundstücks- und Pachtverhältnis

## Definition

Vertrags- und Nutzungsdaten zu kommunalen Grundstücks- und Pachtverhältnissen.

## Felder

- Grundstück
- Vertragspartner
- Vertragsart
- Laufzeit
- Entgelt
- Nutzungszweck

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-10

**Bleibt bei B.** **Vertrags- und Rechtsverhältnis mit der Kommune.** Erfasst werden Vertragspartner, Gegenstand, Laufzeit und Entgelt -- Angaben, die die betroffene Person selbst ausgehandelt hat und die keine Rückschlüsse auf ihre persönlichen Verhältnisse erlauben. Bei juristischen Personen fehlt der Personenbezug ganz; erfasst sind dann nur die vertretungsberechtigten Personen mit dienstlichen Angaben.

**Anzuheben wäre der Speicher, sobald Zahlungsrückstände, Mahnungen oder Kündigungsgründe erfasst werden.** Diese Angaben gehören in `dstore-vollstreckungsdaten` beziehungsweise `dstore-mahnwesen`.

*Sammelvermerk der Durchsicht vom 2026-08-10.*
