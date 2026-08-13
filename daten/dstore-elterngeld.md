---
id: dstore-elterngeld
typ: datenspeicher
system: null
name: Elterngeldantrag
datenkategorie: ''
zuständige-einheit: oe-amt-51
bpmn:
  typ: datenobjekt
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
  - gesetz: BEEG
  aufbewahrung:
    frist: 7 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Elterngeld
- Kind
- Familie
konvertiert-aus: daten1/dtype-elterngeld.md
---



## Beschreibung

Antrag auf Elterngeld nach BEEG.

## Felder

- Antragsteller
- Kind
- Bezugszeitraum
- Einkommensdaten
- Kontodaten

## Rechtsgrundlage

BEEG

## Löschfrist

7 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `normal`** · **Verfügbarkeit: `hoch`**

**Über `normal` gesetzt: Verfügbarkeit `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Integrität bleibt bei `normal`**, geprüft anhand der Fragen des Durchgangs vom 2026-08-04:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

## Schutzstufe geprüft 2026-08-10

**C → D.** Der Antrag nach dem BEEG enthält das **vollständige Erwerbseinkommen der zwölf Monate vor der Geburt** -- nicht eine Momentaufnahme, sondern eine Jahresübersicht mit allen Schwankungen. Aus der Aufteilung der Bezugsmonate zwischen den Eltern und aus dem Verzicht auf Partnermonate lassen sich zudem familiäre Verhältnisse ablesen.

Elterngeld ist eine Sozialleistung nach § 25 Abs. 2 SGB I; die Angaben unterliegen dem Sozialgeheimnis des § 35 SGB I.
