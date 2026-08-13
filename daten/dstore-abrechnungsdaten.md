---
id: dstore-abrechnungsdaten
typ: datenspeicher
system: null
name: Abrechnungsdaten
datenkategorie: Personal & HR
zuständige-einheit: oe-amt-11
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: EStG
  - gesetz: SGB IV
  - gesetz: TVöD
  aufbewahrung:
    frist: 10 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Gehalt
- Abrechnung
- Lohn
- Personal
konvertiert-aus: daten1/dtype-abrechnungsdaten.md
---


## Beschreibung

Gehalts- und Lohnabrechnungsdaten von Mitarbeitern.

## Felder

- Personalnummer
- Abrechnungszeitraum
- Bruttogehalt
- Abzüge
- Nettogehalt
- Steuerklasse

## Rechtsgrundlage

EStG, SGB IV, TVöD

## Löschfrist

10 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** Der Speicher wird in so vielen Verfahren geführt, dass ein Ausfall nicht ein Verfahren verzögert, sondern den Publikumsverkehr insgesamt zum Erliegen bringt. Das ist der Maßstab des BSI: erhebliche Beeinträchtigung der Aufgabenerfüllung.

Die Gehaltsabrechnung ist terminfest; ein Ausfall zum Monatsende trifft alle Beschäftigten.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Beschäftigtendaten mit Bewertungsbezug.** Das LfD-Schutzstufenkonzept nennt dienstliche Beurteilungen ausdrücklich bei Stufe D. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Hinzu kommt das Abhängigkeitsverhältnis:** Beschäftigte können der Verarbeitung nicht ausweichen, und eine Offenlegung innerhalb der Verwaltung wirkt im täglichen Zusammenarbeiten fort. Für die Personalakte gilt zudem § 88 NBG mit einem eigenen Zugriffsregime, das strenger ist als das allgemeine Datenschutzrecht.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
