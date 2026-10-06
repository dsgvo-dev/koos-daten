---
id: dstore-personalstammdaten-beschaeftigte
bereich: intern
typ: datenspeicher
system: null
name: Personalstammdaten der Beschäftigten
zuständige-einheit: oe-amt-11
personenbezug: ja
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. b und lit. c, Art. 88
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  - gesetz: NBG
    artikel: § 88 Abs. 1, § 94 Abs. 1
  - gesetz: EStG
    artikel: § 39e
  - gesetz: SGB IV
    artikel: § 28a
  aufbewahrung:
    frist: 5 Jahre
    beginn: nach Abschluss der Personalakte
    hinweis: 'Frist der Personalakte nach § 94 Abs. 1 NBG; gilt nach § 12 Abs. 1 NDSG auch für Tarifbeschäftigte.'
letzte-aktualisierung: '2026-10-05'
tags:
- Personal
- Stammdaten
- Beschäftigtendaten
- D1
---

# Personalstammdaten der Beschäftigten

## Definition

Grunddaten der Beschäftigten der Kommune (Beamtinnen und Beamte, Tarifbeschäftigte, Auszubildende, Praktikantinnen und Praktikanten, Bundesfreiwilligendienst), wie sie die Personalstelle für Bezüge, Steuer- und Sozialversicherungsmeldungen und die Beihilfe führt. Beschäftigtenspeicher nach Entscheidung D1 vom 05.10.2026.

## Felder

- Personalnummer
- Name, Vorname, Geburtsdatum
- Anschrift
- private Kontaktdaten
- Familienstand
- Kinder (Familienzuschlag, Kinderkomponente)
- Bankverbindung für die Bezüge
- Steuer-Identifikationsnummer
- Sozialversicherungsnummer

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). Die Personalverwaltung nutzte bis dahin Bürger-Speicher: `dstore-personenstammdaten`, `dstore-personenstammdaten-vertraulich`, `dstore-kontaktdaten`, `dstore-bankverbindung`, `dstore-bankverbindung-vertraulich`, `dstore-familienstand-ehebezug`, `dstore-kindergeldbezug`.

**Bewerbende nicht hier.** Nach D1 stehen sie im Bewerberspeicher `dstore-bewerbungsunterlagen` und werden bei Einstellung übernommen.

**Schutzstufe D.** 11-002 und 11-014 sind vertrauliche Verfahren und nutzten die vertraulichen Varianten auf Stufe D; nach dem Maximalprinzip (Skill vvt-datenspeicher, R6) gilt D für den Speicher.

**BSI-Vektoren.** Vertraulichkeit hoch. Integrität hoch: Fehler in Bankverbindung, Steuer- oder Sozialversicherungsdaten führen zu Fehlzahlungen und falschen Meldungen an Finanzamt und Sozialversicherung. Verfügbarkeit normal.

**Abgrenzung:**
- `dstore-personalakte`: Inhalte der Personalakte (Ernennung, Beurteilungen, Qualifikationen).
- `dstore-abrechnungsdaten`: Gehalts- und Lohnabrechnung.
- `dstore-personenstammdaten`, `dstore-personenstammdaten-vertraulich`: Bürgerinnen und Bürger in Verwaltungsverfahren, extern.
