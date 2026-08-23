---
id: dstore-auskunftssperre-melderegister
typ: datenspeicher
system: null
name: Auskunftssperre Melderegister
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: E
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: sehr hoch
  bsi-integritaet: sehr hoch
  bsi-verfuegbarkeit: sehr hoch
  bsi-schutzbedarf: sehr hoch
  rechtsgrundlagen:
  - gesetz: BMG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Auskunftssperre
- Melderegister
- Schutz
---



# Auskunftssperre Melderegister

## Definition

Sperrvermerk zum Schutz gefährdeter Personen im Melderegister.

## Felder

- Betroffene Person
- Sperrgrund
- Anordnende Behörde
- Gültigkeitszeitraum
- Prüffrist
- Aktenbezug

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## Einstufung nach dem Maximalprinzip 2026-08-03

**Von C auf E.** Eine Auskunftssperre nach § 51 BMG wird eingerichtet, wenn Tatsachen die
Annahme rechtfertigen, dass der betroffenen Person durch eine Melderegisterauskunft eine
**Gefahr für Leben, Gesundheit, persönliche Freiheit** oder ähnliche schutzwürdige
Interessen droht. Das ist wortgleich das Kriterium der Stufe E im Schutzstufenkonzept des
LfD Niedersachsen.

Die Sperre existiert, weil eine konkrete Gefährdung festgestellt wurde. Ein Datenabfluss
aus diesem Speicher trifft genau die Personen, die am wenigsten davon vertragen -- Opfer
häuslicher Gewalt, bedrohte Zeuginnen und Zeugen, Personen in Zeugenschutzmaßnahmen.

Damit ist dies der dritte Speicher der Stufe E, neben
`dstore-anmeldebescheinigung-prostschg` und `dstore-hiv-beratung-pseudonym`.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `sehr hoch`** · **Verfügbarkeit: `sehr hoch`**

**Über `normal` gesetzt: Integrität `sehr hoch` und Verfügbarkeit `sehr hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei E.** Die Einstufung wurde am 2026-08-04 bei der Anlage beziehungsweise
Überarbeitung dieses Speichers ausführlich begründet -- siehe die Hinweise oben. Der
Durchgang vom 2026-08-10 hat sie bestätigt und trägt hier nur den Prüfvermerk nach, der bisher
fehlte.

*Der Vermerk ist kein Formalismus: Ohne ihn zählte der Speicher als ungeprüft, und der
Rückstand wies 129 statt der tatsächlich offenen 115 Speicher aus -- allesamt auf Stufe C.*
