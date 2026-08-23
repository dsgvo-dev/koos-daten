---
id: dstore-vergabe-auftragsbezug
typ: datenspeicher
system: null
name: Vergabe- und Auftragsbezug
zuständige-einheit: oe-amt-10
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
  - gesetz: VgV
  - gesetz: UVgO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-04'
tags:
- Vergabe
- Auftrag
- Leistung
---



# Vergabe- und Auftragsbezug

## Definition

Daten zum Bezug einer Rechnung oder Zahlung auf Vergabe- und Auftragsvorgänge.

## Felder

- Vergabenummer
- Auftragnehmer/in
- Leistungsbeschreibung
- Bestelldatum
- Auftragswert
- Rechnungsbezug

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

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

## Schutzstufe geprüft 2026-08-14

**C bestätigt.** Der Auftragswert ist bei natürlichen Personen (Einzelunternehmer,
Freiberufler) eine Einkommensangabe und berührt die wirtschaftlichen Verhältnisse. Die
Art.-10-Daten (Führungszeugnis, Gewerbezentralregisterauskunft) sind in
`dstore-fuehrungszeugnis` und `dstore-register-und-zuverlaessigkeitsauskuenfte` (beide D)
ausgelagert — dieser Speicher führt nur den Auftragsbezug.

Geprüft im Rahmen der Schutzstufendurchsicht Los 4 (Amt 10). Vorschlag:
`_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-14-los4-amt10.md`.

