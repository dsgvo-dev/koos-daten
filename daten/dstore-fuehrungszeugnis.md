---
id: dstore-fuehrungszeugnis
typ: datenspeicher
system: null
name: Führungszeugnis
datenkategorie: Ordnung & Sicherheit
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: BZRG
  aufbewahrung:
    frist: 3 Monate
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Führungszeugnis
- Unbescholtenheit
- Polizei
konvertiert-aus: daten1/dtype-fuehrungszeugnis.md
---



## Beschreibung

Polizeiliches Führungszeugnis zum Nachweis der Unbescholtenheit.

## Felder

- Antragsteller
- Verwendungszweck
- Ausstellungsdatum
- Inhalt

## Rechtsgrundlage

BZRG

## Löschfrist

3 Monate

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

**Schutzstufe angehoben 2026-08-04: C → D.** Das LfD-Schutzstufenkonzept nennt
Straffälligkeit ausdrücklich als D-Beispiel. Der Speicher führt den Inhalt eines
Führungszeugnisses und offenbart strafrechtliche Verurteilungen — das sind Daten
nach Art. 10 DSGVO. Die vorige Einstufung C war unzutreffend. Dass dieser Speicher
bisher C trug, ist der Grund dafür, dass das Prüfskript bei Art.-10-Fällen im
gesamten Bestand keinen D/E-Speicher findet: 15 Verarbeitungstätigkeiten führen
diesen Speicher, viele davon mit Art.-10-Bezug, und die Schutzstufe war zu
niedrig.

**Hinweis für die TOM-Ableitung:** Ein Führungszeugnis ist nicht nur nach seiner
Stufe zu schützen. § 72a Abs. 5 SGB VIII verbietet für die Jugendhilfe ausdrücklich
die Speicherung des Zeugnisses selbst und beschränkt die Datenerhebung auf drei
Felder (Umstand der Einsichtnahme, Datum, Ergebnis). Diese Beschränkung ist eine
TOM-Frage, keine Stufenfrage — aber sie setzt voraus, dass der Speicher, der den
Inhalt des Zeugnisses enthält, überhaupt erkennbar macht, *warum* er besonders
geschützt ist. Die Stufe D stellt das sicher.

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

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Straffälligkeit, Verdacht und Zuverlässigkeitsprüfung.** Das LfD-Schutzstufenkonzept nennt Straffälligkeit bei Stufe D; Art. 10 DSGVO stellt Daten über strafrechtliche Verurteilungen und Straftaten unter einen eigenen Vorbehalt. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Der Verdacht wiegt hier so schwer wie die Feststellung.** Wird bekannt, dass gegen jemanden ermittelt wird, wirkt das unabhängig vom Ausgang -- die spätere Einstellung erreicht selten dieselben Personen wie der ursprüngliche Vorwurf.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
