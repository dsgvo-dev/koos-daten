---
id: dstore-verstorbenenhinweis-melderegister
typ: datenspeicher
system: null
name: Verstorbenenhinweis im Melderegister
datenkategorie: Register- und Nachweisdaten
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: BMG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- verstorben
- Melderegister
- Status
---

# Verstorbenenhinweis im Melderegister

## Definition

Status- und Hinweisdaten, mit denen im Melderegister der Tod einer Person oder ein entsprechender Hinweis verarbeitet wird.

## Felder

- Sterbestatus
- Sterbedatum
- Hinweisquelle
- Mitteilungsdatum
- Bemerkung

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: datenspeicher

## Rechtsgrundlagen

- BMG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Melderegisterauskunft, einfach, Beantragung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
