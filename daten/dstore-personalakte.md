---
id: dstore-personalakte
typ: datenspeicher
system: null
name: Personalakte
zuständige-einheit: oe-amt-11
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: sehr hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: sehr hoch
  rechtsgrundlagen:
  - gesetz: NBG
  - gesetz: TVöD
  - gesetz: DSGVO
  aufbewahrung:
    frist: 10 Jahre nach Ausscheiden
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Personal
- Mitarbeiter
- HR
konvertiert-aus: daten1/dtype-personalakte.md
---



## Beschreibung

Vollständige Personalakte eines Mitarbeiters der Kommunalverwaltung.

## Felder

- Personalnummer
- Name
- Stelle
- Einstellungsdatum
- Qualifikationen
- Beurteilungen

## Rechtsgrundlage

NBG, TVöD, DSGVO

## Löschfrist

10 Jahre nach Ausscheiden

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

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

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Beschäftigtendaten mit Bewertungsbezug.** Das LfD-Schutzstufenkonzept nennt dienstliche Beurteilungen ausdrücklich bei Stufe D. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Hinzu kommt das Abhängigkeitsverhältnis:** Beschäftigte können der Verarbeitung nicht ausweichen, und eine Offenlegung innerhalb der Verwaltung wirkt im täglichen Zusammenarbeiten fort. Für die Personalakte gilt zudem § 88 NBG mit einem eigenen Zugriffsregime, das strenger ist als das allgemeine Datenschutzrecht.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
