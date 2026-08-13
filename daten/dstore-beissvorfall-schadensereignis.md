---
id: dstore-beissvorfall-schadensereignis
typ: datenspeicher
system: null
name: Beißvorfall und Schadensereignis
datenkategorie: Tiere & Haltung
zuständige-einheit: oe-amt-32
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
  - gesetz: NHundG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-04'
tags:
- Beißvorfall
- Schaden
- Hund
---


# Beißvorfall und Schadensereignis

## Definition

Sachverhaltsdaten zu einem gemeldeten Angriff oder Beißvorfall durch einen Hund.

## Felder

- Ereignisdatum
- Ereignisort
- geschädigte Person oder Tier
- Hergang
- Verletzungsart
- Meldende Person

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- NHundG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Angriff Hund melden (Beißvorfall)

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## Schutzstufe geprüft 2026-08-04

Geprüft im Zuge der Auflösung von `vvt-61-001` und `vvt-61-002`: Alle Speicher mit
Freitextfeldern wurden gegen das Schutzstufenkonzept des LfD Niedersachsen gehalten.
Maßstab ist das Maximalprinzip -- die sensibelste Angabe, die anfallen **kann**.

Die entscheidende Frage lautet: **Schreibt die betroffene Person selbst hinein, oder
formuliert eine Fachstelle?** Ist der Text von außen frei bestimmbar, ist mit Angaben nach
Art. 9 Abs. 1 DSGVO zu rechnen. Formuliert eine Behörde sachbezogen, ist er es nicht.

**Von C auf D.** Ein Beißvorfall wird gemeldet, weil ein Mensch oder ein Tier verletzt wurde. Die Meldung enthält damit **Angaben über Verletzungen einer namentlich bekannten Person** -- Gesundheitsdaten nach Art. 9 Abs. 1 DSGVO. Das ist keine mögliche Nebenfolge, sondern der Inhalt der Meldung.

Betroffen sind zwei Personen mit gegenläufigen Interessen: die gebissene und die haltende. Beide Datenbestände sind zu trennen; die haltende Person hat keinen Anspruch darauf, die Verletzungsfolgen im Einzelnen zu erfahren, soweit sie nicht zur Verteidigung erforderlich sind.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** Der Bestand wird in einer Gefahrenlage gebraucht, in der es auf Minuten ankommt. Ein Ausfall bedeutet, dass die Kommune die Lage nicht einschätzen kann.

Die Meldung löst Sofortmaßnahmen aus; die Verletzungsversorgung und die Gefahrenabwehr hängen daran.
