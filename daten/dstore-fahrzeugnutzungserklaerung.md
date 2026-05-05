---
id: dstore-fahrzeugnutzungserklaerung
typ: datenspeicher
system: null
name: Fahrzeugnutzungserklärung
datenkategorie: Fahrzeug- und Mobilitätsdaten
zuständige-einheit: oe-amt-34
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: StVO
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Fahrzeug
- Nutzungserklärung
- Parkausweis
---

# Fahrzeugnutzungserklärung

## Definition

Erklärung, dass ein Fahrzeug dauerhaft von der antragstellenden Person genutzt wird.

## Felder

- Nutzungsberechtigte Person
- Fahrzeughalter
- Kennzeichen
- Beginn Nutzung
- Erklärungsdatum
- Unterschrift

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- StVO

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Bewohnerparkausweis, Erst- und Folgeausstellung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
