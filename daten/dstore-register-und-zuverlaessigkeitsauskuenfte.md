---
id: dstore-register-und-zuverlaessigkeitsauskuenfte
typ: datenspeicher
system: null
name: Register- und Zuverlässigkeitsauskünfte
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenspeicher
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
  - gesetz: BZRG
  - gesetz: GewO
  - gesetz: verfahrensabhängig
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-10'
tags:
- Führungszeugnis
- Gewerbezentralregister
- Schuldnerverzeichnis
- FAER
- Zuverlässigkeit
---



# Register- und Zuverlässigkeitsauskünfte

## Definition

Behördliche Auskünfte und Registerauszüge zur Prüfung persönlicher oder gewerberechtlicher Zuverlässigkeit.

## Felder

- Führungszeugnis
- Gewerbezentralregisterauszug
- Auskunft aus dem Schuldnerverzeichnis
- FAER-Auszug
- Steuerunbedenklichkeitsbescheinigung

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: vertraulich
- BPMN-Typ: datenspeicher

## Rechtsgrundlagen

- BZRG
- GewO
- verfahrensabhängig

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Führungszeugnis, einfach, Beantragung
- Spielhallen, Erlaubnis
- Veranstaltung eines Jahr- oder Spezialmarktes: Festsetzung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Die Auskünfte wurden zu einem Sammeltyp dedupliziert, da sie in mehreren Erlaubnisverfahren wiederkehren.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** Der Speicher wird in so vielen Verfahren geführt, dass ein Ausfall nicht ein Verfahren verzögert, sondern den Publikumsverkehr insgesamt zum Erliegen bringt. Das ist der Maßstab des BSI: erhebliche Beeinträchtigung der Aufgabenerfüllung.

10 Verwendungen in gewerblichen Erlaubnisverfahren, die unter Bearbeitungsfristen stehen.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Straffälligkeit, Verdacht und Zuverlässigkeitsprüfung.** Das LfD-Schutzstufenkonzept nennt Straffälligkeit bei Stufe D; Art. 10 DSGVO stellt Daten über strafrechtliche Verurteilungen und Straftaten unter einen eigenen Vorbehalt. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Der Verdacht wiegt hier so schwer wie die Feststellung.** Wird bekannt, dass gegen jemanden ermittelt wird, wirkt das unabhängig vom Ausgang -- die spätere Einstellung erreicht selten dieselben Personen wie der ursprüngliche Vorwurf.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
