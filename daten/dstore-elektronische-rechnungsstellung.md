---
id: dstore-elektronische-rechnungsstellung
typ: datenspeicher
system: null
name: Elektronische Rechnungsstellung
datenkategorie: Finanzen & E-Government
zuständige-einheit: oe-amt-20
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
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: NDIG
    artikel: § 6 Abs. 3 i. V. m. § 3 Abs. 6
  - gesetz: NERechVO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-04'
tags:
- Rechnung
- Elektronisch
- XRechnung
---



# Elektronische Rechnungsstellung

## Definition

Strukturierte Daten einer elektronischen Rechnung an die Kommune.

## Felder

- Rechnungsnummer
- Rechnungsdatum
- Leitweg-ID
- Betrag
- Leistungsempfänger
- Format

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `hoch`** · **Verfügbarkeit: `hoch`**

**Über `normal` gesetzt: Integrität `hoch` und Verfügbarkeit `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

## Schutzstufe geprüft 2026-08-13

**C bestätigt.** Eine XRechnung nach EN 16931 führt Name, Anschrift und Steuermerkmale des
Ausstellers als Pflichtfelder — der Personenbezug ist dem Gegenstand zwingend, auch wenn die
Feldliste der Datei ihn nicht aufzählt. Rechtsgrundlage: § 6 Abs. 3 NDIG i. V. m. NERechVO
(statt ERechV, korrigiert).

Geprüft im Rahmen der Schutzstufendurchsicht Los 3 (Amt 20). Vorschlag:
`_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-13-los3-amt20-korrigiert.md`.

