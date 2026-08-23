---
id: dstore-person
typ: datenspeicher
system: null
name: Person
zuständige-einheit: oe-amt-33
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
  - gesetz: DSGVO
    artikel: Art. 6
  - gesetz: NDSG
    artikel: § 3
  aufbewahrung:
    frist: Kontextabhängig
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Person
- Name
- Geburtsdatum
konvertiert-aus: daten1/dtype-person.md
---


## Beschreibung

Grundlegende Personendaten: Name, Vorname, Geburtsdatum, Geburtsort.

## Felder

- Familienname
- Vorname
- Geburtsdatum
- Geburtsort
- Geschlecht

## Rechtsgrundlage

Art. 6 DSGVO, § 3 NDSG

## Löschfrist

Kontextabhängig

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-10

**Bleibt bei B.** **Identifikations- und interne Verwaltungsdaten.** Name, Kontaktdaten und der Nachweis, dass eine dienstliche Formalie erledigt ist. Die Angaben sind für die betroffene Person nicht belastend; ihre Preisgabe beeinträchtigt weder die gesellschaftliche Stellung noch die wirtschaftlichen Verhältnisse.

**Das gilt ausdrücklich nur für die Datenschutz-Schutzstufe.** Bei `dstore-it-berechtigungsantrag` und `dstore-schluesselverwaltung` liegt die Brisanz in der Informationssicherheit -- beide stehen dort seit dem 2026-08-04 auf hoher Integrität und hoher Verfügbarkeit. Die beiden Maßstäbe messen Verschiedenes, und das ist hier gut zu sehen.

*Sammelvermerk der Durchsicht vom 2026-08-10.*
