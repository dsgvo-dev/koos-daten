---
id: dstore-brandschutznachweis
typ: datenspeicher
system: null
name: Brandschutznachweis
datenkategorie: Bauen & Grundstück
zuständige-einheit: oe-amt-37
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: NBauO
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-04'
tags:
- Brandschutz
- Nachweis
- Gebäude
---


# Brandschutznachweis

## Definition

Nachweisdaten zu brandschutzrechtlichen Anforderungen eines Bauvorhabens.

## Felder

- Brandschutzkonzept
- erstellende Person
- Prüfdatum
- Gebäudeklasse
- Maßnahmen
- Unterlagenverweis

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- NBauO

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Baugenehmigung Erteilung
- Nutzungsänderung von Gebäuden, Genehmigung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## Schutzstufe geprüft 2026-08-14

**C bestätigt.** Brandschutzkonzept und Gebäudedaten sind sachbezogen. Die erstellende Person ist eine Berufsangabe, kein sensibles personenbezogenes Datum. Keine Art. 9-Daten. C ist angemessen.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit hoch.** Der Bestand dient der Gefahrenabwehr. Ist er verfälscht oder im entscheidenden Moment nicht abrufbar, kann die Kommune ihre Schutzaufgabe nicht erfüllen -- mit möglichen Folgen für Leib und Leben.

Der Nachweis ist Grundlage der Genehmigung und wird im Einsatzfall herangezogen.
