---
id: dstore-arbeitsunfaehigkeit-krankheit
typ: datenspeicher
system: null
name: Arbeitsunfähigkeit und Krankheit
datenkategorie: Gesundheit & Soziales
zuständige-einheit: oe-amt-53
bpmn:
  typ: nachricht
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: SGB V
  - gesetz: BEEG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-10'
tags:
- Arbeitsunfähigkeit
- Krankheit
- Bescheinigung
---



# Arbeitsunfähigkeit und Krankheit

## Definition

Nachweise über krankheitsbedingte Arbeitsunfähigkeit oder gesundheitliche Einschränkungen, soweit sie verfahrensrelevant sind.

## Felder

- Beginn Arbeitsunfähigkeit
- Ende Arbeitsunfähigkeit
- ärztliche Bescheinigung
- Diagnosehinweis
- Bezug zur Leistung
- Nachweisdatei

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: nachricht

## Rechtsgrundlagen

- SGB V
- BEEG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Elterngeld beantragen
- Hilfe zur Gesundheit

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Gesundheit und andere besondere Kategorien nach Art. 9 DSGVO.** Die Verarbeitung ist grundsätzlich untersagt und nur zulässig, wenn ein Ausnahmetatbestand des Art. 9 Abs. 2 DSGVO greift. Das LfD-Schutzstufenkonzept ordnet diese Angaben der Stufe D zu; die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Praktische Folge:** Für diese Speicher ist der Zugriff auf die Personen zu beschränken, die ihn zur Aufgabenerfüllung brauchen -- eine amtsärztliche Stellungnahme gehört nicht in die allgemeine Personalakte, sondern in einen gesondert geführten Teilbestand.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
