---
id: dstore-tk-teilnehmerdaten
bereich: intern
typ: datenspeicher
system: null
name: Teilnehmerdaten Telekommunikationsanlage
zuständige-einheit: oe-amt-15
bpmn:
  typ: datenspeicher
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
  - gesetz: Art. 88 DSGVO i.V.m. § 12 NDSG
  - gesetz: Dienstvereinbarung Telekommunikationsanlagen (reg-dv-telefonie)
  aufbewahrung:
    frist: bis Abmeldung des Anschlusses
    beginn: Ausscheiden oder Wechsel der Nebenstelle
letzte-aktualisierung: '2026-09-30'
tags:
- Telefonie
- Teilnehmerverzeichnis
- Beschäftigte
---

# Teilnehmerdaten Telekommunikationsanlage

## Definition

Zuordnung der Beschäftigten zu ihren Nebenstellen. Grundlage des internen
Teilnehmerverzeichnisses, das die Telefonzentrale pflegt (Prozess Schritt 05).

## Felder

- Name
- Vorname
- Nebenstellennummer
- Kostenstelle
- Organisationszugehörigkeit

## Rechtsgrundlage

Art. 88 DSGVO i.V.m. § 12 NDSG; Dienstvereinbarung Telekommunikationsanlagen
(`reg-dv-telefonie`), § 9 Abs. 1.

## Löschfrist

Bis zur Abmeldung des Anschlusses (Ausscheiden oder Wechsel der Nebenstelle).

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Schutzstufe geprüft 2026-09-30

**B.** Dienstliche Erreichbarkeitsdaten, nicht frei zugänglich; eine unsachgemäße
Handhabung lässt keine besondere Beeinträchtigung erwarten (Beispiel „Verteiler“
im Schutzstufenkonzept). Nicht A, weil die Beschäftigten die Daten nicht selbst
veröffentlicht haben.

*Quelle: `vvt-1-5-001` (Datenkategorie „Stammdaten“), `reg-dv-telefonie` § 9 Abs. 1.*
