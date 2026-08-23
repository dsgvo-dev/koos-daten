---
id: dstore-hundesteuermarke
typ: datenspeicher
system: null
name: Hundesteuermarke
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: kommunale Satzung
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-12'
tags:
- Hundesteuer
- Steuermarke
- Hund
---


# Hundesteuermarke

## Definition

Ausgabe- und Zuordnungsdaten zu einer Hundesteuermarke.

## Felder

- Markennummer
- Ausgabedatum
- zugeordneter Hund
- Halter
- Status aktiv/inaktiv
- Rückgabedatum

## Klassifizierung

- Schutzstufe: B
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- kommunale Satzung

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Hundehaltung Anmeldung
- Hundesteuer – Erhebung

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

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** Markennummer, Ausgabedatum, zugeordneter Hund, Halter, Status, Rückgabedatum.

Die Marke hängt sichtbar am Halsband.

**Zur Abgrenzung von den übrigen Steuerdaten.** Steuerdaten fallen sonst unter C, weil sie die wirtschaftlichen Verhältnisse offenbaren — das LfD-Schutzstufenkonzept nennt die Grundsteuer als Beispiel. Die Hundesteuer ist ein satzungsmäßiger Pauschalbetrag je Hund; aus ihr lässt sich nichts über Einkommen oder Vermögen ableiten. Der Marke fehlt der Bezug zur Leistungsfähigkeit, der die Einstufung der übrigen Steuerdaten trägt.

Die Haltung eines Hundes ist ein nach außen sichtbarer Alltagsvorgang. Für die *gewöhnliche* Hundehaltung trägt keine dieser Datenarten eine Beeinträchtigung der betroffenen Person.

**Abgrenzung.** `dstore-erlaubnis-gefaehrlicher-hund` und `dstore-maulkorb-leinenanordnung` bleiben bei C. Dort belegt der Eintrag einen ordnungsrechtlichen Vorgang gegen die Halterin — die Feststellung der Gefährlichkeit nach § 7 NHundG. Der Unterschied ist nicht der Hund, sondern der Verwaltungsakt.

**Lücke im Verzeichnis:** `verwendungen: 0`. Als eigener Auftrag vorgemerkt.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
