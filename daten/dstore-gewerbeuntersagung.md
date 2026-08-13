---
id: dstore-gewerbeuntersagung
typ: datenspeicher
system: null
name: Gewerbeuntersagung und Unzuverlässigkeit
datenkategorie: Gewerbe & Betrieb
zuständige-einheit: oe-amt-32
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
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c
  - gesetz: DSGVO
    artikel: Art. 10
  - gesetz: GewO
    artikel: § 35
  - gesetz: GewO
    artikel: § 149
  - gesetz: NDSG
    artikel: § 17
  aufbewahrung:
    frist: nach den Tilgungsfristen des § 153 GewO
    beginn: mit Eintragung in das Gewerbezentralregister
    hinweis: '§ 153 GewO: Tilgung nach drei bis fünf Jahren je nach Entscheidung.
      Nach Tilgung darf die Untersagung nicht mehr verwertet werden.'
letzte-aktualisierung: '2026-08-10'
tags:
- Gewerberecht
- Untersagung
- Art. 10 DSGVO
---


# Gewerbeuntersagung und Unzuverlässigkeit

## Definition

Unterlagen eines Gewerbeuntersagungsverfahrens nach § 35 GewO einschließlich der Tatsachen, auf die die Unzuverlässigkeit gestützt wird.

## Felder

- Gewerbetreibende Person
- Gewerbeart und Betriebsstätte
- Untersagungsgrund
- Auskunft aus dem Schuldnerverzeichnis
- Steuerrückstände und Sozialversicherungsbeiträge
- Auskunft aus dem Gewerbezentralregister
- Anhörung und Stellungnahme
- Untersagungsverfügung mit Datum
- Eintragung in das Gewerbezentralregister
- Tilgungsdatum nach § 153 GewO

## Hinweise

Angelegt am 2026-08-03 zu `vvt-32-011` (Gewerberecht).

**Stufe D.** Die Unzuverlässigkeit nach § 35 GewO wird regelmäßig auf wirtschaftliche Leistungsunfähigkeit gestützt -- Eintragungen im Schuldnerverzeichnis, Steuerrückstände, rückständige Sozialversicherungsbeiträge. Das Schutzstufenkonzept des LfD nennt Schulden ausdrücklich als Beispiel der Stufe D. Kommen strafrechtliche Verurteilungen hinzu, tritt Art. 10 DSGVO daneben.

**Die Untersagung entzieht die wirtschaftliche Existenzgrundlage.** Das ist der Maßstab, an dem sich der Umgang mit diesen Daten messen lassen muss.

**Das Tilgungsdatum ist ein eigenes Feld.** Nach § 153 GewO darf eine getilgte Untersagung der betroffenen Person nicht mehr vorgehalten werden. Ohne ein Feld, das den Zeitpunkt führt, ist das Verwertungsverbot nicht umsetzbar -- derselbe Grund wie beim Disziplinarvorgang.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Der Bestand ist Grundlage einer Entscheidung über einen Menschen. Eine unbemerkte Verfälschung führt zu einer falschen Entscheidung, die für die betroffene Person unmittelbare Folgen hat und im Nachhinein kaum aufzuklären ist.

Die Untersagung entzieht die wirtschaftliche Existenzgrundlage und wird ins Gewerbezentralregister eingetragen.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Straffälligkeit, Verdacht und Zuverlässigkeitsprüfung.** Das LfD-Schutzstufenkonzept nennt Straffälligkeit bei Stufe D; Art. 10 DSGVO stellt Daten über strafrechtliche Verurteilungen und Straftaten unter einen eigenen Vorbehalt. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Der Verdacht wiegt hier so schwer wie die Feststellung.** Wird bekannt, dass gegen jemanden ermittelt wird, wirkt das unabhängig vom Ausgang -- die spätere Einstellung erreicht selten dieselben Personen wie der ursprüngliche Vorwurf.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
