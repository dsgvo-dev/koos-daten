---
id: dstore-identitaetsnachweis
typ: datenspeicher
system: null
name: Identitätsnachweis
datenkategorie: Identitätsdaten
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: PAuswG
  - gesetz: PassG
  - gesetz: DSGVO
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-04-09'
tags:
- Personalausweis
- Reisepass
- eID
- Passersatz
- Legitimation
---

# Identitätsnachweis

## Definition

Daten aus amtlichen Identitätsdokumenten zur Legitimation der antragstellenden, vertretenen oder erklärenden Person.

## Felder

- Dokumentart
- Dokumentnummer
- Vorname
- Familienname
- Gültigkeitsdatum
- ausstellende Behörde
- eID-Nutzung

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- PAuswG
- PassG
- DSGVO

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Urkunde, Geburtsurkunde/Geburtenregister, Beantragung
- Geburt, Anzeige
- Dokumente und Kopien: Beglaubigung
- Vorläufige Dokumente, Beantragung
- Personalausweis Beantragung
- Reisepass Beantragung
- Elterngeld, Antrag

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Der Typ deckt sowohl Ausweisdaten als auch Passdaten ab; biometrische Elemente sind separat ausgelagert.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.
