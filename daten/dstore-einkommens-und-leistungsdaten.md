---
id: dstore-einkommens-und-leistungsdaten
typ: datenspeicher
system: null
name: Einkommens- und Leistungsdaten
datenkategorie: Sozialleistungsdaten
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeit: streng vertraulich
  rechtsgrundlagen:
  - gesetz: BEEG
  - gesetz: SGB
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Einkommen
- Elterngeld
- Mutterschaftsgeld
- Zuschuss
- Einnahmen
---

# Einkommens- und Leistungsdaten

## Definition

Finanz- und Leistungsdaten zur Prüfung von Ansprüchen in sozialrechtlichen Verfahren.

## Felder

- Erwerbseinkommen im Bemessungszeitraum
- voraussichtliches Erwerbseinkommen im Bezugszeitraum
- Mutterschaftsgeld
- Arbeitgeberzuschuss
- sonstige Einnahmen
- Nachweiszeitraum

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BEEG
- SGB

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Elterngeld, Antrag

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Nur aufgenommen, wenn im Portal explizit als Unterlagen- oder Nachweiskategorie genannt.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
