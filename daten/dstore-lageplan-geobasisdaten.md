---
id: dstore-lageplan-geobasisdaten
typ: datenspeicher
system: null
name: Lageplan und Geobasisdaten
datenkategorie: Bauen & Grundstück
zuständige-einheit: oe-amt-62
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
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: NBauO
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-04'
tags:
- Lageplan
- LGLN
- Geobasisdaten
---


# Lageplan und Geobasisdaten

## Definition

Plan- und Kartengrundlagen zur räumlichen Einordnung eines Bauvorhabens.

## Felder

- Lageplan
- Maßstab
- Ausfertigungsdatum
- vermessende Stelle
- Koordinatenbezug
- Grundstücksbezug

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
- Genehmigungsfreie Baumaßnahmen Mitteilung
- Antrag auf Verlängerung der Geltungsdauer

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*
