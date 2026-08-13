---
id: dstore-sozialdaten
typ: datenspeicher
system: null
name: Sozialdaten
datenkategorie: Soziales & Jugend
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: sehr hoch
  bsi-verfuegbarkeit: sehr hoch
  bsi-schutzbedarf: sehr hoch
  rechtsgrundlagen:
  - gesetz: SGB I
  - gesetz: SGB II
  - gesetz: SGB XII
  - gesetz: BDSG
  aufbewahrung:
    frist: 10 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Sozialleistung
- SGB
- Hilfe
konvertiert-aus: daten1/dtype-sozialdaten.md
---



## Beschreibung

Personenbezogene Daten im Rahmen von Sozialleistungsverfahren nach SGB.

## Felder

- Leistungsart
- Bedarfsgemeinschaft
- Einkommensverhältnisse
- Vermögen
- Hilfebedarf

## Rechtsgrundlage

SGB I, SGB II, SGB XII, BDSG

## Löschfrist

10 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

**Schutzstufe angehoben 2026-08-04: C → D.** Das LfD-Schutzstufenkonzept nennt
Sozialdaten ausdrücklich als D-Beispiel. Der Speicher führt Leistungsart,
Bedarfsgemeinschaft, Einkommensverhältnisse, Vermögen und Hilfebedarf — sämtlich
existenzrelevant. Die vorige Einstufung C war eine Voreinstellung aus der
Konvertierung; Sozialdaten sind nach R6 und dem LfD-Konzept zwingend D.

Diese Anhebung betrifft 14 Verarbeitungstätigkeiten. Da es sich um die Korrektur
einer dokumentierten Voreinstellung handelt, ist keine Einzelprüfung jeder
Verwendung erforderlich — der Speicher hätte nie C tragen dürfen.

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

**Bleibt bei D.** **Wirtschaftliche Notlage und Sozialleistungsbezug.** Das LfD-Schutzstufenkonzept nennt Sozialdaten, Schulden und Pfändungen ausdrücklich bei Stufe D; § 35 SGB I stellt Sozialdaten zusätzlich unter das Sozialgeheimnis. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Der gemeinsame Nenner ist die Wirkung:** Wird bekannt, dass jemand Leistungen bezieht, Mietschulden hat oder gepfändet wird, beeinträchtigt das die gesellschaftliche Stellung und den Zugang zu Wohnung, Kredit und Arbeit erheblich.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
