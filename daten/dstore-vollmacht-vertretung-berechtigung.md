---
id: dstore-vollmacht-vertretung-berechtigung
typ: datenspeicher
system: null
name: Vollmacht, Vertretung und Berechtigungsnachweis
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: BGB
  - gesetz: verfahrensabhängig
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-12'
tags:
- Vollmacht
- Vertretung
- Berechtigung
- gesetzlicher Vertreter
- Einverständniserklärung
---


# Vollmacht, Vertretung und Berechtigungsnachweis

## Definition

Nachweise, dass eine Person für eine andere handeln darf oder berechtigt ist, Informationen oder Dokumente zu erhalten.

## Felder

- Vollmachtgeber
- bevollmächtigte Person
- gesetzlicher Vertreter
- Einverständniserklärung
- Umfang der Vertretung
- Unterschrift

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BGB
- verfahrensabhängig

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Urkunde, Geburtsurkunde/Geburtenregister, Beantragung
- Dokumente und Kopien: Beglaubigung
- Vorläufige Dokumente, Beantragung
- Führungszeugnis, einfach, Beantragung
- Spielhallen, Erlaubnis

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Rechtliches Interesse und gesetzliche Vertretung wurden hier mit klassischer Vollmacht zusammengeführt.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Der Bestand entscheidet darüber, wer für eine andere Person handeln darf. Eine verfälschte Vollmacht ermöglicht Handlungen gegen deren Willen.

## Schutzstufe geprüft 2026-08-12

**Bleibt bei C.** Vollmachtgeber, bevollmächtigte Person, gesetzlicher Vertreter,
Einverständniserklärung, Umfang der Vertretung.

Verwendet in `vvt-33-001` (Melderegisterauskunft durch Bevollmächtigte) und `vvt-53-004`
(Einsichtnahme in Todesbescheinigungen durch Angehörige).

**Geprüft und verworfen wurde eine Anhebung auf D.** Das Feld „gesetzlicher Vertreter" kann
eine rechtliche Betreuung anzeigen und damit mehr offenbaren als eine gewöhnliche Vollmacht.
Der Speicher führt jedoch die Vertretungsbefugnis, nicht ihren Grund; ein gesetzlicher
Vertreter ist im Regelfall ein sorgeberechtigter Elternteil. Für D fehlt die medizinische
oder soziale Angabe, die das LfD-Konzept dort verlangt.

*Durchsicht Los 2 (Amt 33) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los2-amt33.md`.*
