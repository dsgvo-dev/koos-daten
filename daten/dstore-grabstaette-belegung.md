---
id: dstore-grabstaette-belegung
typ: datenspeicher
system: null
name: Grabstätte, Nutzungsrecht und Belegung
zuständige-einheit: oe-amt-66
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
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. b, lit. c und lit. e
  - gesetz: Nds. BestattG
  - gesetz: Kommunale Friedhofssatzung
  aufbewahrung:
    frist: bis zum Ablauf des Nutzungsrechts, danach 10 Jahre
    beginn: nach Ablauf oder Rückgabe des Nutzungsrechts
    hinweis: Die längere Vorhaltung dient der Klärung von Nutzungsrechten bei Rückfragen
      von Angehörigen; Festlegung des Trägers.
letzte-aktualisierung: '2026-08-04'
tags:
- Friedhof
- Bestattung
- Nutzungsrecht
---


# Grabstätte, Nutzungsrecht und Belegung

## Definition

Zuordnung von Grabstätten zu Nutzungsberechtigten und Verstorbenen einschließlich Belegung, Laufzeit und Pflegevereinbarungen.

## Felder

- Grabstättenbezeichnung (Feld, Reihe, Nummer)
- Grabart
- Nutzungsberechtigte Person
- Laufzeit des Nutzungsrechts
- Bestattete Person mit Geburts- und Sterbedatum
- Datum der Bestattung
- Art der Bestattung einschließlich Einäscherung
- Pflegevereinbarung

## Hinweise

Angelegt am 2026-08-03 zu `vvt-66-001` (Friedhofsverwaltung).

Die VVT führte Personen- und Sterbedaten, aber keinen Speicher für die Grabstätte selbst -- den Kern der Friedhofsverwaltung. Auch „Krematoriumsdienste" standen im Titel ohne jede Datenart; die Einäscherung ist hier als Bestattungsart erfasst.

**Nutzungsberechtigte und Verstorbene sind zu trennen.** Die verstorbene Person fällt nicht unter die DSGVO, die nutzungsberechtigte schon. Die Grablage ist über den Friedhof öffentlich sichtbar; die Zuordnung zur nutzungsberechtigten Person ist es nicht.

## Schutzstufe geprüft 2026-08-14

**C bestätigt.** Die Grablage ist über den Friedhof öffentlich sichtbar. Die Zuordnung zur nutzungsberechtigten Person ist personenbezogen, aber kein Art. 9-Datum. Verstorbene fallen nicht unter die DSGVO. Die Art der Bestattung (Einäscherung) ist eine persönliche Entscheidung ohne sensible Zusatzoffenbarung. C ist angemessen.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*
