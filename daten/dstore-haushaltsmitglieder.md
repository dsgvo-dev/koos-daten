---
id: dstore-haushaltsmitglieder
typ: datenspeicher
system: null
name: Haushaltsmitglieder und Haushaltsgröße
datenkategorie: Wohnen & Soziales
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenobjekt
kontext:
  rolle: basis
  kontextabhaengig: true
  varianten:
  - id: dstore-haushaltsmitglieder-vertraulich
    bedingung: verfahren-vertraulich
  regelquelle: regeln/kontextregeln.yaml
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
  - gesetz: WoGG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-04'
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

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-14

**Bleibt bei C.** Die Haushaltszusammensetzung — wer mit wem zusammenlebt, Verwandtschaftsverhältnis, Geburtsdatum — offenbart familiäre und wirtschaftliche Verhältnisse (C-Kriterium). Das LfD-Schutzstufenkonzept ordnet die Offenbarung familiärer Verhältnisse der Stufe C zu, soweit sie nicht in einem Hilfe-/Leistungskontext steht; für den vertraulichen Kontext gibt es seit 2026-08-14 `dstore-haushaltsmitglieder-vertraulich` (D).

Der Speicher ist bewusst allgemein gehalten. Seine vier bisherigen Verwendungen lagen allerdings ausschließlich in vertraulichen Verfahren und werden deshalb auf die Kontextvariante umgehängt (siehe unten). Die Basis bleibt für nicht-vertrauliche Verwendungen — etwa das Wohngeldverfahren — bestehen.

## Aufspaltung 2026-08-14: allgemeine und vertrauliche Variante

**Dieser Speicher deckt ab 2026-08-14 nur noch die Routineverfahren ab.** Die Haushaltsdaten einer Person im Wohngeldverfahren und die einer Person in der Jugendhilfe — dieselbe Datenart, ein anderer Aussagegehalt.

Die Durchsicht (Los 6) hatte ergeben, dass der Speicher ausschließlich in vier vertraulichen Verfahren geführt wurde (Sozialhilfe SGB XII, Jugendhilfe SGB VIII, AsylbLG, Infektionsschutz) und dort „familiäre Verhältnisse" einer hilfesuchenden Person trägt. Statt den allgemeinen Speicher auf D anzuheben, wird die vertrauliche Kontextvariante `dstore-haushaltsmitglieder-vertraulich` (D) geführt.

Alle vier bisherigen Verwendungen sind auf die Kontextvariante umgehängt worden. Die Basis trägt damit derzeit keine aktive Verwendung und bleibt als allgemeine Datenart bestehen.

