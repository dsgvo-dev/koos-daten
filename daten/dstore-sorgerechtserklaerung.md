---
id: dstore-sorgerechtserklaerung
typ: datenspeicher
system: null
name: Sorgeerklärung
datenkategorie: Personenstandsdaten
zuständige-einheit: oe-amt-31
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: BGB
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-10'
tags:
- Sorgeerklärung
- Sorgerecht
- Kind
---



# Sorgeerklärung

## Definition

Erklärungsdaten zum gemeinsamen oder alleinigen Sorgerecht für ein Kind.

## Felder

- Sorgeberechtigte Person
- Erklärungsart
- Beurkundungsdatum
- beurkundende Stelle
- Aktenzeichen
- Wirksamkeitsstatus

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BGB

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Elterngeld beantragen
- Geburt, Unterlagen zur Beurkundung eines Kindes

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** An den Vorgang knüpft eine gesetzliche Frist. Ist der Bestand im entscheidenden Zeitraum nicht abrufbar, läuft die Frist gleichwohl -- mit Rechtsfolgen für die Kommune oder die betroffene Person.

Sie entscheidet darüber, wer für ein Kind handeln darf -- im Eilfall unmittelbar relevant.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Familiäre, aufenthaltsrechtliche und weltanschauliche Verhältnisse.** Anders als bei den am selben Tag herabgestuften Personenstandsspeichern trägt dieser Bestand eine Angabe, die für sich genommen belastend ist -- eine Sorgerechtsentscheidung, die Abstammung, die Religionszugehörigkeit, den Aufenthaltsstatus oder die Ausübung eines Grundrechts. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
