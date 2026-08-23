---
id: dstore-uebermittlungssperre-melderegister
typ: datenspeicher
system: null
name: Übermittlungssperre Melderegister
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: sehr hoch
  bsi-verfuegbarkeit: sehr hoch
  bsi-schutzbedarf: sehr hoch
  rechtsgrundlagen:
  - gesetz: BMG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-12'
tags:
- Übermittlungssperre
- Melderegister
- Widerspruch
---



# Übermittlungssperre Melderegister

## Definition

Widerspruchs- und Sperrdaten zur Datenübermittlung aus dem Melderegister.

## Felder

- Betroffene Person
- Sperrart
- Datum des Widerspruchs
- Umfang
- Registervermerk
- Gültigkeit

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

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

## Schutzstufe geprüft 2026-08-12

**Bleibt bei C.** Eine Herabstufung auf B wurde am selben Tag vorgeschlagen und nach
Gegenlesen **verworfen**. Die Begründung der Verwerfung ist der eigentliche Inhalt dieses
Vermerks, damit der Vorschlag nicht wiederkehrt.

### Was der Speicher führt

Betroffene Person · **Sperrart** · Datum des Widerspruchs · Umfang · Registervermerk ·
Gültigkeit. Datenkategorie: *Melde- & Schutzdaten*.

### Warum nicht B

**Das Feld „Sperrart" ist offen.** Nichts im Datenmodell begrenzt den Speicher auf die
Widerspruchsrechte nach § 50 Abs. 5 BMG. Das Maximalprinzip (R6) verlangt, die sensibelste
Angabe zugrunde zu legen, die anfallen *kann* — nicht die typische. Eine Abgrenzung, die nur
im Vermerk behauptet und nicht im Datenmodell durchgesetzt ist, trägt keine Herabstufung.

**Die bloße Existenz einer Sperre sagt etwas aus.** Wer erfährt, dass für eine Person ein
Sperrvermerk geführt wird, erfährt zweierlei: dass diese Person nicht gefunden werden will,
und dass sie im Bezirk dieser Meldebehörde gemeldet ist. Das ist das Kriterium aus ADR 010 —
es kommt nicht auf den Inhalt der Datenart an, sondern darauf, worüber ihre bloße Existenz
Auskunft gibt.

**Der Verwendungskontext spannt beide Enden.** In `vvt-10-002` (Alters- und Ehejubiläum) ist
es der harmlose Widerspruch nach § 50 Abs. 5 BMG; in `vvt-33-001` (Melderegisterführung) ist
es die Sperrverwaltung insgesamt. Nach R6 Schritt 2 gilt der sensible Kontext.

### Warum nicht D

Die beiden Sachverhalte, bei denen die Existenz einer Sperre eine **Gefährdung** anzeigt,
führt der Bestand in eigenen Speichern der Stufe E, und beide sind in `vvt-33-001`
zusätzlich gesetzt:

- **Auskunftssperre nach § 51 BMG** — Tatsachen begründen die Annahme einer Gefahr für Leben,
  Gesundheit oder persönliche Freiheit → `dstore-auskunftssperre-melderegister` (E)
- **Bedingter Sperrvermerk nach § 52 BMG** — Anschriften von Personen, die in einer
  Pflegeeinrichtung, einer Einrichtung zum Schutz vor häuslicher Gewalt oder einer
  Suchtbehandlungseinrichtung gemeldet sind → `dstore-schutzbeduerftigkeitskennzeichen` (E)

Bleibt für diesen Speicher die Sperrverwaltung unterhalb der Gefährdungsschwelle: mehr als
eine folgenlose Verwaltungsangabe, weniger als eine Existenzgefährdung. Das ist C.

### Nicht als Aufspaltung behandelt

Eine Trennung nach ADR-010-Muster — Basisspeicher für die Widersprüche, Variante für die
Sperrverwaltung — wäre denkbar. Sie wurde nicht vorgenommen, weil der Speicher nur zwei
Verwendungen hat und die beiden E-Speicher die kritischen Fälle bereits abdecken.

*Durchsicht Los 2 (Amt 33) vom 2026-08-12, Korrektur nach Gegenlesen. Grundlage:
`_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los2-amt33.md`.*
