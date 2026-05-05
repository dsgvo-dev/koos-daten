---
id: dstore-register-und-zuverlaessigkeitsauskuenfte
typ: datenspeicher
system: null
name: Register- und Zuverlässigkeitsauskünfte
datenkategorie: Gewerbe & Erlaubnisse
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: BZRG
  - gesetz: GewO
  - gesetz: verfahrensabhängig
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
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
