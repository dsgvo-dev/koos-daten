---
id: dstore-jugendgerichtshilfe-tatvorwurf
typ: datenspeicher
system: null
name: Tatvorwurf in der Jugendgerichtshilfe
zuständige-einheit: oe-amt-51
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
  - gesetz: DSGVO
    artikel: Art. 10
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: NDSG
    artikel: § 17
  - gesetz: SGB VIII
    artikel: § 52
  - gesetz: JGG
    artikel: § 38
  aufbewahrung:
    frist: bis zur Vollendung des 24. Lebensjahres
    beginn: nach Abschluss des Verfahrens
    hinweis: Angelehnt an § 63 Abs. 1 Nr. 3 JGG für die Tilgung im Erziehungsregister.
      Festlegung des Trägers; abweichende Fristen des Bundeszentralregisters bleiben
      unberührt.
letzte-aktualisierung: '2026-08-10'
tags:
- Jugendhilfe
- Art. 10 DSGVO
- Jugendgerichtshilfe
---



# Tatvorwurf in der Jugendgerichtshilfe

## Definition

Angaben über den Gegenstand eines Straf- oder Bußgeldverfahrens gegen Jugendliche oder Heranwachsende, soweit die Jugendgerichtshilfe daran mitwirkt.

## Felder

- Beschuldigte Person
- Aktenzeichen des Verfahrens
- Tatvorwurf und Tatzeitpunkt
- Verfahrensstand
- gerichtlicher Beschluss
- Stellungnahme der Jugendgerichtshilfe
- angeordnete Weisungen oder Arbeitsstunden
- Ableistungsnachweis

## Hinweise

Angelegt am 2026-08-03 zu `vvt-51-012` (Mitwirkung in gerichtlichen Verfahren).

**Datum nach Art. 10 DSGVO, nicht nach Art. 9.** Angaben über Straftaten und strafrechtliche Verurteilungen unterliegen einem eigenen Regime: Sie dürfen nur unter behördlicher Aufsicht oder aufgrund einer besonderen Rechtsvorschrift verarbeitet werden. Die VVT zitierte bisher Art. 9 Abs. 2, aber nicht Art. 10.

**Abgrenzung zu `dstore-bussgeldakte`:** Diese führt kommunale Ordnungswidrigkeitenverfahren. Hier geht es um die Mitwirkung an einem Verfahren, das ein Gericht führt.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Der Bestand ist Grundlage einer Entscheidung über einen Menschen. Eine unbemerkte Verfälschung führt zu einer falschen Entscheidung, die für die betroffene Person unmittelbare Folgen hat und im Nachhinein kaum aufzuklären ist.

Die Stellungnahme geht in ein gerichtliches Verfahren gegen einen jungen Menschen ein.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Straffälligkeit, Verdacht und Zuverlässigkeitsprüfung.** Das LfD-Schutzstufenkonzept nennt Straffälligkeit bei Stufe D; Art. 10 DSGVO stellt Daten über strafrechtliche Verurteilungen und Straftaten unter einen eigenen Vorbehalt. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Der Verdacht wiegt hier so schwer wie die Feststellung.** Wird bekannt, dass gegen jemanden ermittelt wird, wirkt das unabhängig vom Ausgang -- die spätere Einstellung erreicht selten dieselben Personen wie der ursprüngliche Vorwurf.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
