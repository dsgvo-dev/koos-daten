---
id: dstore-disziplinarvorgang
typ: datenspeicher
system: null
name: Disziplinarvorgang
zuständige-einheit: oe-amt-11
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
    artikel: Art. 10
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. b
  - gesetz: NDSG
    artikel: § 17
  - gesetz: NDiszG
  - gesetz: NBG
    artikel: § 88
  aufbewahrung:
    frist: nach den Tilgungsfristen des § 24 NDiszG
    beginn: mit Abschluss des Verfahrens
    hinweis: '§ 24 NDiszG: Verweis nach zwei Jahren, Geldbuße und Kürzung der Bezüge
      nach drei Jahren, Zurückstufung nach sieben Jahren zu tilgen. Nach Tilgung darf
      der Vorgang nicht mehr verwertet werden.'
letzte-aktualisierung: '2026-08-10'
tags:
- Disziplinarrecht
- Art. 10 DSGVO
- Personal
---


# Disziplinarvorgang

## Definition

Unterlagen eines Disziplinarverfahrens gegen Beamtinnen und Beamte einschließlich der Ermittlungen und der Disziplinarmaßnahme.

## Felder

- Betroffene Beamtin oder Beamter
- Aktenzeichen
- Vorwurf und Sachverhalt
- Ermittlungsergebnis
- Disziplinarmaßnahme
- Datum der Unanfechtbarkeit
- Tilgungsdatum nach § 24 NDiszG
- Verwertungsverbot vermerkt

## Hinweise

Angelegt am 2026-08-03 zu `vvt-11-002` (Arbeits- und Dienstverhältnisse).

**Getrennt von der Personalakte zu führen.** Die Datenkategorien der VVT vermerkten „ggf. Disziplinarakte separat" -- das ist zutreffend und folgt aus § 88 NBG in Verbindung mit dem NDiszG. Ein eigener Speicher macht die Trennung im Verzeichnis sichtbar.

**Datum nach Art. 10 DSGVO.** Disziplinarvorwürfe betreffen Dienstvergehen, die zugleich Straftaten sein können; die Rechtsprechung behandelt Disziplinardaten wie Daten über Straftaten. Das LfD-Konzept nennt Straffälligkeit und dienstliche Beurteilungen ausdrücklich als Beispiele der Stufe D.

**Das Verwertungsverbot ist ein Feld, keine Fußnote.** Nach Tilgung darf der Vorgang bei künftigen Entscheidungen nicht mehr berücksichtigt werden. Ohne ein Feld, das den Tilgungszeitpunkt führt, ist das nicht umsetzbar.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Der Bestand ist Grundlage einer Entscheidung über einen Menschen. Eine unbemerkte Verfälschung führt zu einer falschen Entscheidung, die für die betroffene Person unmittelbare Folgen hat und im Nachhinein kaum aufzuklären ist.

Der Vorgang trägt Maßnahmen bis zur Entfernung aus dem Dienst und unterliegt Tilgungsfristen nach § 24 NDiszG. Eine unbemerkte Änderung kann die Tilgung unterlaufen.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Straffälligkeit, Verdacht und Zuverlässigkeitsprüfung.** Das LfD-Schutzstufenkonzept nennt Straffälligkeit bei Stufe D; Art. 10 DSGVO stellt Daten über strafrechtliche Verurteilungen und Straftaten unter einen eigenen Vorbehalt. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Der Verdacht wiegt hier so schwer wie die Feststellung.** Wird bekannt, dass gegen jemanden ermittelt wird, wirkt das unabhängig vom Ausgang -- die spätere Einstellung erreicht selten dieselben Personen wie der ursprüngliche Vorwurf.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
