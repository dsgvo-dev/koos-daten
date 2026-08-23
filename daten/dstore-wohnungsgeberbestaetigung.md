---
id: dstore-wohnungsgeberbestaetigung
typ: datenspeicher
system: null
name: Wohnungsgeberbestätigung
zuständige-einheit: oe-amt-33
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
  - gesetz: BMG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-12'
tags:
- Wohnungsgeber
- Einzug
- Wohnung
- Melderecht
---


# Wohnungsgeberbestätigung

## Definition

Nachweis über den Bezug einer Wohnung zur Anmeldung oder Ummeldung bei der Meldebehörde.

## Felder

- Name Wohnungsgeber
- Anschrift Wohnung
- Einzugsdatum
- Wohnungsart
- Zuordnungsmerkmal
- Bestätigungserteilung

## Klassifizierung

- Schutzstufe: B
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BMG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Hauptwohnsitz anmelden
- Wohnsitz Anmeldung
- Wohnsitz Abmeldung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Sie ist nach § 19 BMG Voraussetzung der Anmeldung; eine gefälschte Bestätigung ermöglicht eine Scheinanmeldung -- § 19 Abs. 6 BMG stellt das ausdrücklich unter Verbot.

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** **§ 19 BMG** verpflichtet den Wohnungsgeber, den Einzug
gegenüber der Meldebehörde zu bestätigen. Die Bestätigung enthält Name und Anschrift des
Wohnungsgebers, das Einzugsdatum, die Anschrift der Wohnung und die Namen der
meldepflichtigen Personen.

Sie belegt ein Mietverhältnis. Das beeinträchtigt weder die gesellschaftliche Stellung noch
die wirtschaftlichen Verhältnisse — anders als etwa Mietschulden, die im Bestand einen
eigenen Speicher auf D haben (`dstore-mietschulden-wohnraumsicherung`).

*Durchsicht Los 2 (Amt 33) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los2-amt33.md`.*
