---
id: dstore-staatsangehoerigkeit-aufenthaltsstatus
typ: datenspeicher
system: null
name: Staatsangehörigkeit und Aufenthaltsstatus
datenkategorie: Identitätsdaten
zuständige-einheit: oe-amt-47
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: AufenthG
  - gesetz: PStG
  - gesetz: BEEG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Staatsangehörigkeit
- Aufenthaltstitel
- Ausland
- Ehefähigkeitszeugnis
---

# Staatsangehörigkeit und Aufenthaltsstatus

## Definition

Daten zur Staatsangehörigkeit, ausländerrechtlichen Stellung und grenzüberschreitenden Personenstandsbezügen.

## Felder

- Staatsangehörigkeit
- Nachweis der Staatsangehörigkeit
- Aufenthaltstitel
- Auslandsbezug
- ausländische Urkunde

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- AufenthG
- PStG
- BEEG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Eheschließung, Anmeldung
- Ehefähigkeitszeugnis, Ausstellung
- Beantragung der Befreiung von der Vorlage des Ehefähigkeitszeugnisses
- Sterbefall im Ausland
- Elterngeld, Antrag

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Ausländische Urkunden und Aufenthaltstitel wurden nicht auf Dokumentenebene, sondern als Status- und Nachweiskategorie zusammengeführt.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
