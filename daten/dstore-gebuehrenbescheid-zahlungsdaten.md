---
id: dstore-gebuehrenbescheid-zahlungsdaten
typ: datenspeicher
system: null
name: Gebührenbescheid und Zahlungsdaten
datenkategorie: Finanzen & Zahlung
zuständige-einheit: oe-amt-20
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: VwKostR
  - gesetz: Kommunalabgabenrecht
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-04'
tags:
- Gebühr
- Bescheid
- Zahlung
---


# Gebührenbescheid und Zahlungsdaten

## Definition

Bescheid- und Zahlungsdaten zu Gebühren im Verwaltungsverfahren.

## Felder

- Gebührenart
- Betrag
- Bescheiddatum
- Fälligkeit
- Kassenzeichen
- Zahlungsstatus

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- VwKostR
- Kommunalabgabenrecht

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Geburtsurkunde beantragen
- Eheurkunde beantragen
- Baugenehmigung Erteilung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** Der Speicher wird in so vielen Verfahren geführt, dass ein Ausfall nicht ein Verfahren verzögert, sondern den Publikumsverkehr insgesamt zum Erliegen bringt. Das ist der Maßstab des BSI: erhebliche Beeinträchtigung der Aufgabenerfüllung.

16 Verwendungen. Kassengeschäft und Vollstreckung setzen den Zugriff voraus.
