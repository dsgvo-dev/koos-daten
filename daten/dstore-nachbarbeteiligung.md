---
id: dstore-nachbarbeteiligung
typ: datenspeicher
system: null
name: Nachbarbeteiligung
zuständige-einheit: oe-amt-63
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: normal
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: NBauO
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-10'
tags:
- Nachbarn
- Bauvorhaben
- Beteiligung
---


# Nachbarbeteiligung

## Definition

Daten zur Benachrichtigung oder Beteiligung von Nachbarinnen und Nachbarn in Bauverfahren.

## Felder

- Nachbargrundstück
- Eigentümer
- Anschrift
- Beteiligungsdatum
- Einwendung
- Ergebnis

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- NBauO

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Baugenehmigung Erteilung
- Außenwerbung, Genehmigung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-10

**C → D.** Das Feld **Einwendung** ist ein Freitext, und die Kommune kann ihn nicht begrenzen: § 68 Abs. 2 NBauO gibt der Nachbarschaft ein Beteiligungsrecht, und eine formularmäßige Verengung würde es verkürzen. Damit gilt dieselbe Überlegung wie bei `dstore-stellungnahme-planverfahren`.

Was in einer Nachbareinwendung steht, reicht von der Abstandsflächenrüge bis zur Schilderung einer Erkrankung, die durch Verschattung oder Lärm verschlimmert wird, und bis zu Vorwürfen aus einem laufenden Nachbarschaftskonflikt. Nach dem Maximalprinzip ist die sensibelste Angabe maßgeblich, die anfallen kann.

**Der Schutz setzt bei der Weitergabe an:** Die Einwendung geht der Bauherrschaft im Rahmen der Anhörung zu. Das ist unvermeidbar, aber die Verwaltung sollte darauf hinwirken, dass persönliche Angaben, die zur Rechtsverteidigung nicht erforderlich sind, nicht mitübersandt werden.
