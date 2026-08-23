---
id: dstore-einkommensdaten
typ: datenspeicher
system: null
name: Einkommensdaten
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: SGB II
  - gesetz: SGB XII
  - gesetz: EStG
  aufbewahrung:
    frist: 10 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-04'
tags:
- Einkommen
- Gehalt
- Lohn
konvertiert-aus: daten1/dtype-einkommensdaten.md
---



## Beschreibung

Einkommensnachweise und Gehaltsdaten für Sozialleistungen und Förderungen.

## Felder

- Einkommensart
- Betrag
- Zeitraum
- Arbeitgeber
- Steuerklasse

## Rechtsgrundlage

SGB II, SGB XII, EStG

## Löschfrist

10 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## Schutzstufe geprüft 2026-08-04

Durchsicht des Katalogs gegen das Schutzstufenkonzept des LfD Niedersachsen,
Maximalprinzip.

**Von C auf D.** Das Schutzstufenkonzept des LfD nennt **Sozialdaten ausdrücklich als Beispiel der Stufe D**. Schon die Existenz eines Eintrags offenbart, dass die betroffene Person eine Sozialleistung bezieht oder beantragt hat -- unabhängig davon, welche Felder gefüllt sind.

Einkommen allein wäre nach dem LfD-Konzept Stufe C. Dieser Speicher ist aber ausdrücklich beschrieben als „Einkommensnachweise und Gehaltsdaten **für Sozialleistungen und Förderungen**" und wird in neun Verarbeitungstätigkeiten geführt, darunter Grundsicherung nach SGB XII (`vvt-50-001`), Unterhaltsvorschuss (`vvt-51-008`) und Vollstreckung (`vvt-21-001`). In diesem Kontext ist die Einkommensangabe zugleich ein Sozialdatum.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `hoch`** · **Verfügbarkeit: `normal`**

**Über `normal` gesetzt: Integrität `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Verfügbarkeit bleibt bei `normal`**, geprüft anhand der Fragen des Durchgangs vom 2026-08-04:

1. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

