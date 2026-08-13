---
id: dstore-bescheid
typ: datenspeicher
system: null
name: Bescheid
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
  - gesetz: VwGO
  aufbewahrung:
    frist: 10 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-04'
tags:
- Bescheid
- Verwaltungsakt
- Entscheidung
konvertiert-aus: daten1/dtype-bescheid.md
---



## Beschreibung

Verwaltungsrechtliche Entscheidung einer Behörde (Genehmigung, Ablehnung, Auflagen).

## Felder

- Bescheidnummer
- Datum
- Empfänger
- Entscheidung
- Begründung
- Rechtsbehelfsbelehrung

## Rechtsgrundlage

NVwVfG, VwGO

## Löschfrist

10 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## Schutzstufe geprüft 2026-08-04

Geprüft im Zuge der Auflösung von `vvt-61-001` und `vvt-61-002`: Alle Speicher mit
Freitextfeldern wurden gegen das Schutzstufenkonzept des LfD Niedersachsen gehalten.
Maßstab ist das Maximalprinzip -- die sensibelste Angabe, die anfallen **kann**.

Die entscheidende Frage lautet: **Schreibt die betroffene Person selbst hinein, oder
formuliert eine Fachstelle?** Ist der Text von außen frei bestimmbar, ist mit Angaben nach
Art. 9 Abs. 1 DSGVO zu rechnen. Formuliert eine Behörde sachbezogen, ist er es nicht.

**Bleibt bei C.** Das Feld „Begründung" könnte grundsätzlich alles aufnehmen. Der Speicher wird aber nur mit ausdrücklichem Beleg gesetzt (Regel R3) und steht derzeit in vier Verarbeitungstätigkeiten: Museumswesen, Sportförderung, öffentliche Bekanntmachungen sowie Bürgerbeteiligung und Petitionen. In keiner davon ergeht ein Bescheid über Gesundheit, Sozialleistungen oder Straftaten.

**Diese Einstufung ist an die Verwendung gebunden.** Wird der Speicher künftig in einem Sozialleistungs- oder Gesundheitsverfahren gesetzt, ist sie neu zu prüfen. Der Regelfall bleibt: In solchen Verfahren gehört ein fachspezifischer Speicher gesetzt, nicht der generische.

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

