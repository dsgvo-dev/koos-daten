---
id: dstore-meldeschein
typ: datenspeicher
system: null
name: Meldeschein
datenkategorie: Wohnen & Melderecht
zuständige-einheit: oe-amt-33
bpmn:
  typ: nachricht
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
  - gesetz: BMG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-12'
tags:
- Meldeschein
- Meldeformular
- Anmeldung
---


# Meldeschein

## Definition

Formular- und Erklärungsdaten, die bei An-, Um- oder Abmeldung eines Wohnsitzes erfasst werden.

## Felder

- Meldedatum
- bisherige Anschrift
- neue Anschrift
- Einzugsdatum
- Wohnstatus
- Unterschrift

## Klassifizierung

- Schutzstufe: B
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: nachricht

## Rechtsgrundlagen

- BMG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Hauptwohnsitz anmelden
- Wohnsitz Abmeldung

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

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** Meldedatum, bisherige und neue Anschrift, Einzugsdatum,
Wohnstatus, Unterschrift — das Formular zur Anmeldung nach § 17 Abs. 1 BMG.

Inhaltlich ist das die Anschrift in Formularform. Die einfache Melderegisterauskunft nach **§ 44 BMG** gibt Familienname, Vornamen, Doktorgrad und die derzeitige Anschrift an jedermann heraus — ohne dass ein berechtigtes Interesse darzulegen wäre. Erst die erweiterte Auskunft nach § 45 BMG verlangt eines.

Folgt damit `dstore-meldeadresse-wohnsitz` und `dstore-adresse`, beide B.

*Durchsicht Los 2 (Amt 33) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los2-amt33.md`.*
