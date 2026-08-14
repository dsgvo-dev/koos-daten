---
id: dstore-genehmigung
typ: datenspeicher
system: null
name: Genehmigung
datenkategorie: Verwaltungsakte & Dokumente
zuständige-einheit: oe-amt-30
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: NVwVfG
  - gesetz: je nach Fachrecht
  aufbewahrung:
    frist: Dauerhaft
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-04'
tags:
- Genehmigung
- Erlaubnis
- Zulassung
konvertiert-aus: daten1/dtype-genehmigung.md
---



## Beschreibung

Behördliche Genehmigung für eine beantragte Tätigkeit oder Maßnahme.

## Felder

- Genehmigungsnummer
- Datum
- Genehmigungsinhaber
- Gegenstand
- Auflagen
- Gültigkeit

## Rechtsgrundlage

NVwVfG, je nach Fachrecht

## Löschfrist

Dauerhaft

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## Schutzstufe geprüft 2026-08-14

**C bestätigt.** Genehmigungsinhaber (Name) und Gegenstand sind Standard-Personendaten im Verwaltungsakt. Der Datenspeicher selbst enthält keine Art. 9-Merkmale. C ist angemessen.

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

