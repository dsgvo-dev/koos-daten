---
id: dstore-verdachtsmeldung-geldwaesche
typ: datenspeicher
system: null
name: Verdachtsmeldung nach Geldwäschegesetz
datenkategorie: Ordnung & Sicherheit
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
  bsi-integritaet: normal
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 10
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c
  - gesetz: GwG
    artikel: § 43
  - gesetz: GwG
    artikel: § 50
  aufbewahrung:
    frist: 5 Jahre
    beginn: nach Abgabe der Meldung
    hinweis: § 8 Abs. 4 GwG.
letzte-aktualisierung: '2026-08-10'
tags:
- Geldwäsche
- GwG
- Art. 10 DSGVO
---



# Verdachtsmeldung nach Geldwäschegesetz

## Definition

Meldung eines Geldwäscheverdachts an die Zentralstelle für Finanztransaktionsuntersuchungen sowie die aufsichtlichen Prüfungsfeststellungen, die zu ihr geführt haben.

## Felder

- Meldende Stelle
- Verpflichtete oder verpflichteter Betrieb
- Sachverhalt und Verdachtsgründe
- betroffene Transaktion
- Datum der Meldung an die FIU
- Prüfungsfeststellungen
- Rückmeldung der FIU

## Hinweise

Angelegt am 2026-08-03 zu `vvt-32-016` (Maßnahmen nach Geldwäschegesetz).

**Datum nach Art. 10 DSGVO.** Ein Geldwäscheverdacht ist ein Verdacht auf eine Straftat nach § 261 StGB.

**Das Verbot der Informationsweitergabe nach § 47 GwG** ist bei der Ausgestaltung der Zugriffsrechte zu beachten: Die betroffene Person darf von der Meldung nichts erfahren. Das schließt die Auskunft nach Art. 15 DSGVO insoweit aus (§ 47 Abs. 1 GwG, Art. 23 DSGVO).

**Abgrenzung zu `dstore-hinweismeldung`:** Diese betrifft die interne Meldestelle nach § 11 HinSchG. Verschiedene Verfahren, verschiedene Empfänger.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `normal`** · **Verfügbarkeit: `hoch`**

**Über `normal` gesetzt: Verfügbarkeit `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Integrität bleibt bei `normal`**, geprüft anhand der Fragen des Durchgangs vom 2026-08-04:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.

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
