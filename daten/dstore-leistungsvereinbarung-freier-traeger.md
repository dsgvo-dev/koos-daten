---
id: dstore-leistungsvereinbarung-freier-traeger
typ: datenspeicher
system: null
name: Leistungsvereinbarung mit freien Trägern
zuständige-einheit: oe-amt-51
bpmn:
  typ: datenobjekt
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
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. b und lit. e
  - gesetz: SGB VIII
    artikel: § 74
  - gesetz: SGB VIII
    artikel: §§ 78a-78g
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Ende der Vereinbarung
letzte-aktualisierung: '2026-08-10'
tags:
- Jugendhilfe
- Leistungsvereinbarung
- freie Träger
---


# Leistungsvereinbarung mit freien Trägern

## Definition

Vereinbarungen über Leistung, Entgelt und Qualitätsentwicklung mit freien Trägern der Jugendhilfe.

## Felder

- Träger
- Vertretungsberechtigte Person
- Ansprechpartner mit dienstlichen Kontaktdaten
- Leistungsumfang
- Entgeltvereinbarung
- Laufzeit
- Qualitätsentwicklungsvereinbarung

## Hinweise

Angelegt am 2026-08-03 zu `vvt-51-016` (Leistungsvereinbarungen mit freien Trägern).

**Personenbezogen ist hier wenig.** Leistungsumfang und Entgelt betreffen den Träger als juristische Person. Personenbezug entsteht nur über die vertretungsberechtigten Personen und die benannten Ansprechpartner. Das sollte bei der Schutzstufe nicht zu einer Hochstufung führen.

**Kein Vergabeverfahren.** Vereinbarungen nach §§ 78a ff. SGB VIII folgen dem sozialrechtlichen Dreiecksverhältnis, nicht dem Vergaberecht; `dstore-vergabe-auftragsbezug` passt nicht.

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
