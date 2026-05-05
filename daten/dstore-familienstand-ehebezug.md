---
id: dstore-familienstand-ehebezug
typ: datenspeicher
system: null
name: Familienstand und Ehebezug
datenkategorie: Personenstandsdaten
zuständige-einheit: oe-amt-31
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: PStG
  - gesetz: PStV
  - gesetz: BGB
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Ehe
- Lebenspartnerschaft
- Scheidung
- Eheurkunde
- Ehefähigkeit
---

# Familienstand und Ehebezug

## Definition

Daten und Nachweise zum aktuellen oder früheren Familienstand sowie zur Ehefähigkeit.

## Felder

- Familienstand
- Eheurkunde
- Scheidungsurteil
- Ehefähigkeitszeugnis
- Auflösung der Lebenspartnerschaft
- Sterbeurkunde früherer Partner

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- PStG
- PStV
- BGB

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Eheschließung, Anmeldung
- Urkunde, Eheurkunde, Beantragung
- Ehefähigkeitszeugnis, Ausstellung
- Beantragung der Befreiung von der Vorlage des Ehefähigkeitszeugnisses
- Sterbefall im Ausland

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Vorverbindungen, Ehehindernisse und Ehefähigkeitsnachweise wurden zu einem Typ gebündelt.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
