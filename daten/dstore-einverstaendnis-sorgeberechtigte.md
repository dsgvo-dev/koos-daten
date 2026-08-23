---
id: dstore-einverstaendnis-sorgeberechtigte
typ: datenspeicher
system: null
name: Einverständnis der Sorgeberechtigten
zuständige-einheit: oe-amt-51
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
  - gesetz: BGB
  - gesetz: PAuswG
  - gesetz: PassG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-10'
tags:
- Einverständnis
- Sorgeberechtigte
- Minderjährige
---


# Einverständnis der Sorgeberechtigten

## Definition

Erklärungsdaten, mit denen Sorgeberechtigte einer Antragstellung oder Dokumentenausgabe für Minderjährige zustimmen.

## Felder

- sorgeberechtigte Person
- Art der Zustimmung
- Datum
- Dokumentbezug
- Unterschrift
- Nachweis Sorgeberechtigung

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BGB
- PAuswG
- PassG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Personalausweis – Ausstellung für unter 16-Jährige
- Kinderreisedokumente beantragen

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

**C → D.** Die Zustimmung selbst wäre Stufe B. Entscheidend ist das Feld **Nachweis der Sorgeberechtigung**.

Im Regelfall ist das die Geburtsurkunde oder eine Sorgeerklärung nach § 1626a BGB. Steht die elterliche Sorge nur einem Elternteil zu, ist es ein Beschluss des Familiengerichts -- und der dokumentiert, dass dem anderen Elternteil die Sorge entzogen oder übertragen wurde, häufig nach einem Verfahren wegen Kindeswohlgefährdung nach § 1666 BGB. Nach dem Maximalprinzip ist diese Möglichkeit maßgeblich.

Betroffen sind zudem Minderjährige.
