---
id: dstore-geburtsurkunde
typ: datenspeicher
system: null
name: Geburtsurkunde
zuständige-einheit: oe-amt-31
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
  - gesetz: PStG
  - gesetz: PStV
  aufbewahrung:
    frist: 110 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-04'
tags:
- Geburt
- Urkunde
- Personenstand
- Standesamt
konvertiert-aus: daten1/dtype-geburtsurkunde.md
---



## Beschreibung

Personenstandsdokument über die Geburt einer Person.

## Felder

- Name
- Geburtsdatum
- Geburtsort
- Eltern
- Standesamtsnummer

## Rechtsgrundlage

PStG, PStV

## Löschfrist

110 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## Schutzstufe geprüft 2026-08-04

Durchsicht des Katalogs gegen das Schutzstufenkonzept des LfD Niedersachsen,
Maximalprinzip.

**Von C auf D -- aus Konsistenz.** Die Geburtsurkunde führt dieselben Angaben wie `dstore-geburtsdaten-kind`, `dstore-geburtsurkunde-eltern` und `dstore-elternbezug-abstammung`, die sämtlich auf D stehen: Abstammung und Eltern-Kind-Zuordnung.

Der Grund für die hohe Einstufung dieser Gruppe liegt in den Randvermerken des Personenstandsregisters. Sie können eine **Adoption** ausweisen, für die § 1758 BGB ein Offenbarungs- und Ausforschungsverbot anordnet, oder eine Vaterschaftsanfechtung. Eine Geburtsurkunde niedriger einzustufen als die Unterlagen, aus denen sie erstellt wird, wäre nicht begründbar.

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

