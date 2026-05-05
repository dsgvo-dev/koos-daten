---
id: dstore-vollmacht-vertretung-berechtigung
typ: datenspeicher
system: null
name: Vollmacht, Vertretung und Berechtigungsnachweis
datenkategorie: Berechtigungsdaten
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: BGB
  - gesetz: verfahrensabhängig
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Vollmacht
- Vertretung
- Berechtigung
- gesetzlicher Vertreter
- Einverständniserklärung
---

# Vollmacht, Vertretung und Berechtigungsnachweis

## Definition

Nachweise, dass eine Person für eine andere handeln darf oder berechtigt ist, Informationen oder Dokumente zu erhalten.

## Felder

- Vollmachtgeber
- bevollmächtigte Person
- gesetzlicher Vertreter
- Einverständniserklärung
- Umfang der Vertretung
- Unterschrift

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BGB
- verfahrensabhängig

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Urkunde, Geburtsurkunde/Geburtenregister, Beantragung
- Dokumente und Kopien: Beglaubigung
- Vorläufige Dokumente, Beantragung
- Führungszeugnis, einfach, Beantragung
- Spielhallen, Erlaubnis

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Rechtliches Interesse und gesetzliche Vertretung wurden hier mit klassischer Vollmacht zusammengeführt.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
