---
id: dstore-tk-verbindungsdaten
typ: datenspeicher
system: null
name: Verbindungsdaten Telekommunikationsanlage
zuständige-einheit: oe-amt-15
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: Art. 88 DSGVO i.V.m. § 12 NDSG
  - gesetz: § 3 TDDDG
  - gesetz: Dienstvereinbarung Telekommunikationsanlagen (reg-dv-telefonie)
  aufbewahrung:
    frist: 3 Monate
    beginn: nach Ablauf des Abrechnungszeitraums
    hinweis: >-
      Einzelverbindungsnachweise 3 Jahre; Zugriffsprotokolle 12 Monate
      (DV § 9 Abs. 4); Betriebsdaten sofort nach Störungsbeseitigung
      (vvt-1-5-001)
letzte-aktualisierung: '2026-09-30'
tags:
- Telefonie
- Verbindungsdaten
- Gebühren
- Protokoll
- Beschäftigte
---

# Verbindungsdaten Telekommunikationsanlage

## Definition

Daten über dienstliche Verbindungen der Telekommunikationsanlage, einschließlich
der Betriebs- und Revisionsdaten (Störungsmeldungen, Zugriffsprotokolle).
Private Nutzung ist nicht gestattet (DV § 6 Abs. 2); private Verbindungsdaten
entstehen deshalb nicht. Für Sonderanschlüsse (Personalrat,
Schwerbehindertenvertretung, Datenschutzbeauftragter) werden keine
Verbindungsdaten gespeichert (DV § 6 Abs. 4).

## Felder

- Kostenstelle
- Rufnummer des rufenden Nebenanschlusses
- angewählte Rufnummer
- Datum und Uhrzeit (Gesprächsbeginn)
- Gesprächsdauer
- Gebühreneinheiten und Gebührenbetrag
- Art der Verbindung (direkt, umgeleitet, Konferenz)
- Störungsmeldungen
- Zugriffsprotokoll: Datum, Uhrzeit, zugreifende Person, Anlass, Umfang

## Rechtsgrundlage

Art. 88 DSGVO i.V.m. § 12 NDSG; § 3 TDDDG (Fernmeldegeheimnis);
Dienstvereinbarung Telekommunikationsanlagen (`reg-dv-telefonie`) §§ 5, 8, 9.

## Löschfrist

- Verbindungsdaten: 3 Monate nach Ablauf des Abrechnungszeitraums
- Einzelverbindungsnachweise: 3 Jahre
- Zugriffsprotokolle: 12 Monate (DV § 9 Abs. 4)
- Betriebsdaten: sofort nach Störungsbeseitigung

Die Löschung ist auf allen Datenträgern vorzunehmen und zu protokollieren
(DV § 8 Abs. 2). Sie obliegt dem IT-Bereich (DV § 10 Abs. 4).

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

Mit einem Vertrag, der alle Verbindungen pauschal abdeckt (Flatrate), entfällt
der Zweck „Gebührendaten den Kostenträgern zuordnen“ (DV § 5 Abs. 1) für diese
Verbindungen. Es verbleiben technischer Betrieb, Stichproben (DV § 7 Abs. 2)
und Einzelverbindungsnachweise.

## Schutzstufe geprüft 2026-09-30

**C.** Die Daten zeigen, wer wann mit wem wie lange telefoniert hat. Sie
eignen sich zur Verhaltens- und Leistungskontrolle der Beschäftigten — deshalb
Mitbestimmung nach § 67 Abs. 1 Nr. 2 NPersVG. Eine unsachgemäße Handhabung kann
die Stellung der Beschäftigten beeinträchtigen („Ansehen“). Nicht D: keine
Gesprächsinhalte, und die Anschlüsse von Personalrat, Schwerbehindertenvertretung
und Datenschutzbeauftragtem sind ausgenommen.

*Quelle: `vvt-1-5-001` (Datenkategorien „Verbindungsdaten dienstlich“,
„Betriebsdaten“, „Revisionsdaten“), `reg-dv-telefonie` §§ 5, 6, 8, 9.*
