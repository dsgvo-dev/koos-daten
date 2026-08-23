---
id: dstore-sondernutzung-oeffentlicher-raum
typ: datenspeicher
system: null
name: Sondernutzung öffentlicher Raum
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: Straßenrecht
  - gesetz: Ortsrecht
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-12'
tags:
- Sondernutzung
- öffentlicher Raum
- Nutzung
---


# Sondernutzung öffentlicher Raum

## Definition

Daten zu einer erlaubnispflichtigen Nutzung des öffentlichen Straßenraums.

## Felder

- Nutzungsart
- Ort
- Zeitraum
- Fläche
- Sicherungsmaßnahmen
- Gebührenbezug

## Klassifizierung

- Schutzstufe: B
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- Straßenrecht
- Ortsrecht

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Außenwerbung, Genehmigung
- Marktfestsetzung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Die Erlaubnis mit ihren Auflagen entscheidet über die Zulässigkeit der Nutzung und über die Gebühr.

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** Nutzungsart, Ort, Zeitraum, Fläche, Sicherungsmaßnahmen, Gebührenbezug.

Die Sondernutzung ist im Straßenraum sichtbar — der Verkaufsstand, die Außenbestuhlung, das Baugerüst stehen dort. Was jeder Passant sehen kann, beeinträchtigt bei Offenbarung niemanden.

Der Gebührenbezug trägt keine Höherstufung: Die Gebühr bemisst sich nach Fläche und Dauer, nicht nach der Leistungsfähigkeit der Person.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
