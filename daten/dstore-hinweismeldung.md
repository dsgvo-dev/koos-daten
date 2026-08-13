---
id: dstore-hinweismeldung
typ: datenspeicher
system: null
name: Hinweismeldung der internen Meldestelle
datenkategorie: Recht & Compliance
zuständige-einheit: oe-amt-30
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
  - gesetz: HinSchG
    artikel: § 10
  - gesetz: HinSchG
    artikel: §§ 8, 9
  - gesetz: HinSchG
    artikel: § 11
  - gesetz: NHinMeldG
    artikel: §§ 1, 2
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c, Art. 9 Abs. 2 lit. g, Art. 10
  aufbewahrung:
    frist: 3 Jahre
    beginn: nach Abschluss des Verfahrens
    hinweis: Frist aus § 11 Abs. 5 HinSchG. Eine längere Aufbewahrung ist nur zulässig,
      soweit sie zur Erfüllung von Anforderungen nach dem HinSchG oder anderen Rechtsvorschriften
      erforderlich und verhältnismäßig ist -- etwa solange ein Straf- oder Disziplinarverfahren
      anhängig ist. Unbegründete Hinweise werden mit Abschluss der Vorprüfung gelöscht,
      spätestens nach drei Monaten (Festlegung des Trägers).
letzte-aktualisierung: '2026-08-10'
tags:
- Hinweisgeberschutz
- Korruptionsprävention
- Meldestelle
- Vertraulichkeit
---



# Hinweismeldung der internen Meldestelle

## Definition

Dokumentation der bei der internen Meldestelle eingehenden Meldungen nach § 11 HinSchG, einschließlich der Folgemaßnahmen.

## Felder

- Eingangskanal und Eingangszeitpunkt
- Anonymitätsstatus der Meldung
- Identität der hinweisgebenden Person, soweit angegeben
- Identität der von der Meldung betroffenen Person und weiterer genannter Personen
- Sachverhaltsdarstellung
- Vertraulichkeitsvermerk mit dem Kreis der Personen, denen die Identitäten bekannt sind
- Ergebnis der Vorprüfung
- Folgemaßnahmen nach § 18 HinSchG
- Offenlegungsvermerk bei einer Weitergabe nach § 9 HinSchG mit Grund und Empfänger
- Abschluss des Verfahrens und Beginn der Dreijahresfrist

## Hinweise

Angelegt am 2026-07-30 zusammen mit `proc-hinweis-auf-korruption-bearbeiten` und `vvt-30-001`. Im Bestand gab es nichts Passendes; `dstore-beschwerde-anregungsdaten` trifft es nicht, weil dort keine Vertraulichkeitspflicht mitgeführt wird.

**Schutzstufe D, streng vertraulich.** Das ergibt sich nicht aus einer Einschätzung, sondern aus § 8 HinSchG: Die Identität der hinweisgebenden Person darf **ausschließlich** den für die Entgegennahme und für Folgemaßnahmen zuständigen Personen bekannt werden. Ein Zugriffskonzept, das dieser Beschränkung nicht folgt, verletzt das Gesetz.

**Der Vertraulichkeitsvermerk ist ein Feld dieses Speichers.** Ohne festgehaltenen Kreis der Wissensträger lässt sich die Einhaltung des § 8 HinSchG weder steuern noch belegen. Dasselbe gilt für den Offenlegungsvermerk: Jede Weitergabe nach § 9 HinSchG ist ein begründungsbedürftiger Ausnahmefall und wird als solcher dokumentiert.

**Der Anonymitätsstatus ist ein eigenes Feld.** Nach § 16 Abs. 1 Satz 4 HinSchG sollen auch anonym eingehende Meldungen bearbeitet werden. Das Feld verhindert, dass eine anonyme Meldung im weiteren Verlauf ungewollt einer Person zugeordnet wird.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** An den Vorgang knüpft eine gesetzliche Frist. Ist der Bestand im entscheidenden Zeitraum nicht abrufbar, läuft die Frist gleichwohl -- mit Rechtsfolgen für die Kommune oder die betroffene Person.

§ 17 HinSchG bindet die interne Meldestelle an harte Fristen: **Eingangsbestätigung binnen sieben Tagen, Rückmeldung binnen drei Monaten**. Ein Ausfall führt unmittelbar zur Fristverletzung, und die ist bußgeldbewehrt.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Straffälligkeit, Verdacht und Zuverlässigkeitsprüfung.** Das LfD-Schutzstufenkonzept nennt Straffälligkeit bei Stufe D; Art. 10 DSGVO stellt Daten über strafrechtliche Verurteilungen und Straftaten unter einen eigenen Vorbehalt. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Der Verdacht wiegt hier so schwer wie die Feststellung.** Wird bekannt, dass gegen jemanden ermittelt wird, wirkt das unabhängig vom Ausgang -- die spätere Einstellung erreicht selten dieselben Personen wie der ursprüngliche Vorwurf.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
