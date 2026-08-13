---
id: dstore-vaterschaftsanerkennung
typ: datenspeicher
system: null
name: Vaterschaftsanerkennung
datenkategorie: Personenstandsdaten
zuständige-einheit: oe-amt-31
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: BGB
  - gesetz: PStG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-10'
tags:
- Vaterschaft
- Anerkennung
- Kind
---



# Vaterschaftsanerkennung

## Definition

Daten aus Erklärungen oder Nachweisen zur Anerkennung der Vaterschaft.

## Felder

- Vater
- Kind
- Anerkennungsdatum
- beurkundende Stelle
- Aktenzeichen
- Urkundennachweis

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BGB
- PStG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Elterngeld beantragen
- Geburt, Unterlagen zur Beurkundung eines Kindes

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** An den Vorgang knüpft eine gesetzliche Frist. Ist der Bestand im entscheidenden Zeitraum nicht abrufbar, läuft die Frist gleichwohl -- mit Rechtsfolgen für die Kommune oder die betroffene Person.

Die Beurkundung ist häufig eilbedürftig, etwa vor einer Geburt oder für Unterhaltsansprüche.

## Schutzstufe geprüft 2026-08-10

**D → C.** **Personenstandsdaten sind nicht als Gruppe hochsensibel.** Die Durchsicht hat sie einzeln geprüft, statt sie pauschal auf D zu belassen. Auf D bleiben die Speicher, die Abstammung, Sorgerechtsentscheidungen oder die Religionszugehörigkeit führen -- `dstore-personenstand`, `dstore-elternbezug-abstammung`, `dstore-sorgerechtsnachweis`, `dstore-sorgerechtserklaerung` und `dstore-geburtsanzeige-unterlagenpaket`.

Vater, Kind, Anerkennungsdatum, beurkundende Stelle. Die Anerkennung nach § 1592 Nr. 2 BGB zeigt an, dass das Kind nicht in einer Ehe geboren wurde -- eine Angabe über die Familienverhältnisse, die das LfD-Schutzstufenkonzept nicht bei Stufe D führt.

**Anzuheben wäre der Speicher, sobald ein Anfechtungs- oder Feststellungsverfahren nach §§ 1598a, 1600d BGB dokumentiert wird.** Dort geht es um die biologische Abstammung und regelmäßig um einen Konflikt; das gehört in `dstore-elternbezug-abstammung`, der auf D bleibt.
