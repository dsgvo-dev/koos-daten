---
id: dstore-rechnungsadressierung-kommune
typ: datenspeicher
system: null
name: Rechnungsadressierung Kommune
datenkategorie: Finanzen & E-Government
personenbezug: nein   # festgestellt 2026-08-12, siehe Vermerk unten
zuständige-einheit: oe-amt-20
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: NDIG
    artikel: § 6 Abs. 3 i. V. m. § 3 Abs. 6
  - gesetz: NERechVO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-12'
tags:
- Rechnung
- Adressierung
- Kommune
---



# Rechnungsadressierung Kommune

## Definition

Adressierungsdaten der Kommune für den elektronischen Rechnungsempfang.

## Felder

- Organisationseinheit
- Rechnungsadresse
- E-Mail oder Portal
- Leitweg-ID
- Ansprechpartner/in
- Gültigkeit

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

## Personenbezug geprüft 2026-08-12

**Kein Personenbezug.**

Der Speicher führt die Rechnungsanschrift der Kommune je Organisationseinheit — Anschrift,
E-Mail oder Portal, Leitweg-ID, Gültigkeit.

**Das Feld „Ansprechpartner/in" benennt eine natürliche Person, ändert das Ergebnis aber
nicht.** Gemeint ist eine Beschäftigte der Kommune in ihrer dienstlichen Funktion, mit
dienstlicher Anschrift. Sie gehört nicht zu den Betroffenen dieser Verarbeitung: `vvt-20-004`
zählt allein Personen auf der Lieferantenseite auf. Beschäftigtendaten der Kommune werden im
Verzeichnis unter den Personalverarbeitungen des Amtes 11 geführt.

Nach Art. 4 Nr. 1 DSGVO sind personenbezogene Daten alle Informationen, die sich auf
eine identifizierte oder identifizierbare **natürliche Person** beziehen. Maßgeblich ist
nicht, ob ein Feld einen Namen trägt, sondern **wem der Datensatz zuzuordnen ist**.

Dieser Datensatz ist einer **Organisationseinheit der Kommune** zuzuordnen, nicht einer
natürlichen Person.

Die verwendende Verarbeitung bestätigt das aus zwei Richtungen:

- `vvt-20-004` nennt als Betroffene ausdrücklich *„Lieferanten, Dienstleister und deren
  Vertretungsberechtigte/Ansprechpartner:innen"* — also Personen auf der **Lieferantenseite**.
- Dieselbe Verarbeitung führt unter `kategorien_daten` die Formulierung *„Leitweg-ID und
  Peppol-ID; Rechnungsadressierung **je Organisationseinheit**"*.

## Was daraus folgt

**Die Datenschutz-Schutzstufe ist für diesen Speicher gegenstandslos.** Das
LfD-Schutzstufenkonzept bemisst den Schaden für die betroffene Person; wo es keine gibt, ist
nichts zu bemessen.

**Die BSI-Vektoren bleiben und sind hier der eigentliche Maßstab.** Der Schaden trifft die
Kommune, nicht eine Person: Eine verfälschte Kennung leitet Rechnungen fehl. Die Integrität
steht deshalb seit dem 2026-08-04 auf `hoch`, und das bleibt so.

## Schutzstufe entfernt (2026-08-13)

`klassifizierung.schutzstufe` ist ersatzlos entfernt — die Bedingung dafür ist erfüllt:

Der A-Default in `besonderheiten_generator.py` ist beseitigt (ADR 011). Der Generator wertet
`personenbezug` jetzt aus und übergeht diesen Speicher für das Schutzstufen-Maximum. Die
effektive Stufe von `vvt-20-004` bleibt C — sie wird von den übrigen neun personenbezogenen
Datenspeichern getragen.

## Das Feld `personenbezug`

`personenbezug: nein` ist am 2026-08-12 festgestellt worden. Seit dem 2026-08-13 (ADR 011)
wird das Feld von `besonderheiten_generator.py`, `kettenpruefung.py` (E7), `kontextpruefung.py`
und `katalog_generator.py` ausgewertet: Ein Speicher mit `personenbezug: nein` trägt keine
Schutzstufe (Achse 1 entfällt); seine BSI-Vektoren bleiben unverändert wirksam.

*Festgestellt bei der Schutzstufendurchsicht Los 3 (Amt 20) am 2026-08-12. Der Speicher bleibt als Datenspeicher bestehen.*
