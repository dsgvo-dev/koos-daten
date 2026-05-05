---
id: dstore-haushaltsmitglieder
typ: datenspeicher
system: null
name: Haushaltsmitglieder und Haushaltsgröße
datenkategorie: Wohnen & Soziales
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeit: intern
  rechtsgrundlagen:
  - gesetz: WoGG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Haushalt
- Haushaltsmitglieder
- Wohngeld
---

# Haushaltsmitglieder und Haushaltsgröße

## Definition

Daten zu den im Haushalt lebenden Personen und ihrer Anzahl.

## Felder

- Anzahl Haushaltsmitglieder
- Person im Haushalt
- Verwandtschaftsverhältnis
- Geburtsdatum
- Haushaltszugehörigkeit
- Auszugs-/Einzugsdatum

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

- Wohngeld erstmalig oder neu beantragen
- Wesentliche Änderungen für Wohngeld mitteilen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
