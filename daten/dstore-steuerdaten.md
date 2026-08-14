---
id: dstore-steuerdaten
typ: datenspeicher
system: null
name: Steuerdaten
datenkategorie: Finanzen & Steuern
zuständige-einheit: oe-amt-22
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: sehr hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: sehr hoch
  rechtsgrundlagen:
  - gesetz: AO
  - gesetz: GrStG
  - gesetz: GewStG
  aufbewahrung:
    frist: 10 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-04'
tags:
- Steuer
- Grundsteuer
- Gewerbesteuer
konvertiert-aus: daten1/dtype-steuerdaten.md
---



## Beschreibung

Steuerrelevante Daten für kommunale Steuern: Grundsteuer, Gewerbesteuer, Hundesteuer.

## Felder

- Steuernummer
- Steuerart
- Bemessungsgrundlage
- Steuerbescheid
- Fälligkeit

## Rechtsgrundlage

AO, GrStG, GewStG

## Löschfrist

10 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## Schutzstufe geprüft 2026-08-14

**C bestätigt.** Steuerdaten (Grundsteuer, Gewerbesteuer, Hundesteuer) enthalten zwar Bemessungsgrundlagen mit Vermögensbezug (Grundsteuer), aber überwiegend Unternehmensbezug (Gewerbesteuer) ohne betroffene Person i. S. d. DSGVO. Der gemischte Charakter (Gewerbe/Privat) rechtfertigt keine Heraufstufung auf D.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `sehr hoch`** · **Verfügbarkeit: `normal`**

**Über `normal` gesetzt: Integrität `sehr hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Verfügbarkeit bleibt bei `normal`**, geprüft anhand der Fragen des Durchgangs vom 2026-08-04:

1. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

