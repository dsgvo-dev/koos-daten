---
id: dstore-beihilfeakte
bereich: intern
typ: datenspeicher
system: null
name: Beihilfeakte
zuständige-einheit: oe-amt-11
personenbezug: ja
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. b
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  - gesetz: NBG
    artikel: § 88, § 89, § 94 Abs. 2
  - gesetz: NBhVO
    artikel: Niedersächsische Beihilfeverordnung
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Ablauf des Jahres, in dem die Bearbeitung des einzelnen Vorgangs abgeschlossen wurde
    hinweis: 'Frist aus § 94 Abs. 2 Satz 1 NBG für Unterlagen über Beihilfe.'
letzte-aktualisierung: '2026-10-05'
tags:
- Personal
- Beihilfe
- Gesundheitsdaten
- Teilakte
---

# Beihilfeakte

## Definition

Beihilfeunterlagen der Beihilfeberechtigten (Beamtinnen und Beamte, Versorgungsempfangende) und ihrer berücksichtigungsfähigen Angehörigen. Nach § 89 NBG stets als Teilakte geführt und von der übrigen Personalakte getrennt aufbewahrt; Bearbeitung in einer getrennten Organisationseinheit, Zugang nur für deren Beschäftigte.

## Felder

- beihilfeberechtigte Person (Verweis auf Personalnummer)
- berücksichtigungsfähige Angehörige
- Bemessungssatz
- Anträge mit Arzt-, Apotheken- und sonstigen Rechnungen
- aus den Belegen erkennbare Diagnosen und Behandlungen
- private Kranken- und Pflegeversicherung (Tarif, Leistungen)
- Beihilfebescheide und Erstattungsbeträge

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). Die Beihilfe (vvt-11-014) nutzte bis dahin drei Bürger-Speicher: `dstore-gesundheitsdaten`, `dstore-rechnungsdaten`, `dstore-krankenversicherungsbeitraege`. Keiner beschreibt die Teilakte nach § 89 NBG.

**Stammdaten und Bankverbindung nicht hier.** Sie stehen in `dstore-personalstammdaten-beschaeftigte`; die Beihilfeakte enthält nur, was § 89 NBG getrennt verlangt.

**Schutzstufe D, Vertraulichkeitsklasse streng vertraulich.** Gesundheitsdaten nach Art. 9 Abs. 1 DSGVO auch von Angehörigen; § 89 NBG beschränkt den Zugang auf die Beihilfestelle.

**BSI-Vektoren.** Vertraulichkeit hoch. Integrität normal: Belege können erneut vorgelegt werden. Verfügbarkeit normal.

**Abgrenzung:**
- `dstore-gesundheitsdaten`: Gesundheitsdaten in Bürgerverfahren, extern.
- `dstore-krankenversicherungsbeitraege`: Beiträge in Leistungs- und Zuschussverfahren, extern.
- `dstore-personalakte`: übrige Personalakte; die Beihilfeakte ist nach § 89 NBG getrennt.
