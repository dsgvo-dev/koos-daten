---
id: dstore-veranstaltungsteilnahme
typ: datenspeicher
system: null
name: Teilnahme an Veranstaltungen
zuständige-einheit: oe-hvb
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
    artikel: Art. 6 Abs. 1 lit. e
  - gesetz: NKomVG
    artikel: § 62
  aufbewahrung:
    frist: 6 Monate
    beginn: nach der Veranstaltung
    hinweis: Sitzordnung und Verpflegungswünsche werden nach der Veranstaltung nicht
      mehr benötigt. Eine Übernahme in Einladungslisten künftiger Veranstaltungen
      ist eine Zweckänderung und bedarf einer eigenen Grundlage.
letzte-aktualisierung: '2026-08-10'
tags:
- Veranstaltung
- Repräsentation
---


# Teilnahme an Veranstaltungen

## Definition

Angaben zur Teilnahme an einer Veranstaltung einschließlich der Sitzordnung.

## Felder

- Eingeladene Person
- Veranstaltung und Datum
- Zu- oder Absage
- Begleitperson
- Platzierung in der Sitzordnung

## Hinweise

Angelegt am 2026-08-03 zu `vvt-1-001` (Repräsentative Veranstaltungen des Hauptverwaltungsbeamten).

**Ohne Verpflegungspräferenzen.** Der Speicher trug bei der Anlage zunächst ein Feld für
Verpflegungswünsche und war deshalb in Stufe D eingeordnet: „halal", „koscher" oder
„Diabetikerkost" offenbaren die religiöse Überzeugung oder den Gesundheitszustand und sind
damit Daten nach Art. 9 Abs. 1 DSGVO.

**Entscheidung des Trägers vom 2026-08-03: Menüpräferenzen werden nicht erhoben.** Damit
entfällt die Datenart -- und mit ihr der Art.-9-Bezug, die ausdrückliche Einwilligung nach
Art. 9 Abs. 2 lit. a) und die Einstufung in Stufe D. Der Speicher steht jetzt auf B.

Das ist der sauberere Weg: Eine Datenart nicht zu erheben, ist wirksamer als sie zu
erheben und besonders zu schützen. Verpflegung ist ohne personenbezogene Vorerfassung zu
organisieren, etwa durch ein Angebot mehrerer Speisen zur Wahl vor Ort.

**Frist auf sechs Monate belassen.** Sitzordnung und Teilnahmestatus werden nach der
Veranstaltung nicht mehr benötigt. Eine Übernahme in Einladungslisten künftiger
Veranstaltungen ist eine Zweckänderung und bedarf einer eigenen Grundlage.

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
