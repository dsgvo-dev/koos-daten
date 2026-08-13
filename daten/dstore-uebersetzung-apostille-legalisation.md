---
id: dstore-uebersetzung-apostille-legalisation
typ: datenspeicher
system: null
name: Übersetzung, Apostille und Legalisation
datenkategorie: Auslandsbezug & Dokumente
zuständige-einheit: oe-amt-30
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
  - gesetz: VwVfG
  - gesetz: PStG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-04'
tags:
- Übersetzung
- Apostille
- Legalisation
- Ausland
---


# Übersetzung, Apostille und Legalisation

## Definition

Begleit- und Echtheitsnachweise für ausländische Dokumente im deutschen Verwaltungsverfahren.

## Felder

- beeidigte Übersetzung
- Apostille
- Legalisation
- Ausstellungsstaat
- Prüfvermerk
- Beglaubigungsdatum

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- VwVfG
- PStG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Geburt im Ausland beurkunden lassen
- Nachbeurkundung einer im Ausland geschlossenen Ehe beantragen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Die Apostille bestätigt die Echtheit einer ausländischen Urkunde. Ist sie verfälscht, bricht die gesamte Beweiskette.
