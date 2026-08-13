---
id: dstore-staatsangehoerigkeit
typ: datenspeicher
system: null
name: Staatsangehörigkeit
datenkategorie: Person & Identität
zuständige-einheit: oe-amt-33
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
  - gesetz: DSGVO
    artikel: Art. 6
  - gesetz: AufenthG
  - gesetz: StAG
  aufbewahrung:
    frist: Kontextabhängig
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Staatsangehörigkeit
- Aufenthaltstitel
- Migration
konvertiert-aus: daten1/dtype-staatsangehoerigkeit.md
---



## Beschreibung

Staatsangehörigkeit und Aufenthaltsstatus einer Person.

## Felder

- Staatsangehörigkeit
- Aufenthaltsstatus
- Aufenthaltstitel
- Gültigkeitsdauer

## Rechtsgrundlage

Art. 6 DSGVO, AufenthG, StAG

## Löschfrist

Kontextabhängig

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

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

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Familiäre, aufenthaltsrechtliche und weltanschauliche Verhältnisse.** Anders als bei den am selben Tag herabgestuften Personenstandsspeichern trägt dieser Bestand eine Angabe, die für sich genommen belastend ist -- eine Sorgerechtsentscheidung, die Abstammung, die Religionszugehörigkeit, den Aufenthaltsstatus oder die Ausübung eines Grundrechts. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
