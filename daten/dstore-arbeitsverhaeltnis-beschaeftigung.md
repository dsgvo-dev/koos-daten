---
id: dstore-arbeitsverhaeltnis-beschaeftigung
typ: datenspeicher
system: null
name: Arbeitsverhältnis und Beschäftigung
datenkategorie: Arbeit & Einkommen
zuständige-einheit: oe-amt-11
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: BEEG
  - gesetz: WoGG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Arbeit
- Beschäftigung
- Arbeitgeber
---

# Arbeitsverhältnis und Beschäftigung

## Definition

Daten zu bestehenden oder früheren Beschäftigungsverhältnissen für Leistungs- und Antragsverfahren.

## Felder

- Arbeitgeber
- Beschäftigungsbeginn
- Beschäftigungsende
- Wochenstunden
- Beschäftigungsart
- Verdienstnachweis

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BEEG
- WoGG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Elterngeld beantragen
- Wohngeld erstmalig oder neu beantragen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
