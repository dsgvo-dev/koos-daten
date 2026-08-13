---
id: dstore-aenderungsmitteilung-wohngeld
typ: datenspeicher
system: null
name: Änderungsmitteilung Wohngeld
datenkategorie: Wohnen & Soziales
zuständige-einheit: oe-amt-64
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: WoGG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-04'
tags:
- Wohngeld
- Änderung
- Mitteilung
---


# Änderungsmitteilung Wohngeld

## Definition

Mitteilungsdaten zu geänderten persönlichen, wirtschaftlichen oder wohnungsbezogenen Verhältnissen im Wohngeldbezug.

## Felder

- Änderungsart
- Änderungsdatum
- alte Angabe
- neue Angabe
- Mitteilungseingang
- Nachweis

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- WoGG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Wesentliche Änderungen für Wohngeld mitteilen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## Schutzstufe geprüft 2026-08-04

Durchsicht des Katalogs gegen das Schutzstufenkonzept des LfD Niedersachsen,
Maximalprinzip.

**Von C auf D.** Das Schutzstufenkonzept des LfD nennt **Sozialdaten ausdrücklich als Beispiel der Stufe D**. Schon die Existenz eines Eintrags offenbart, dass die betroffene Person eine Sozialleistung bezieht oder beantragt hat -- unabhängig davon, welche Felder gefüllt sind.

Die Mitteilung nennt „geänderte persönliche, wirtschaftliche oder wohnungsbezogene Verhältnisse" -- also Trennung, Arbeitsplatzverlust oder Einkommenseinbruch. Sie ist sensibler als der Antrag selbst, weil sie den Wendepunkt dokumentiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*
