---
id: dstore-zuverlaessigkeitsanfrage-sicherheitsbehoerden
typ: datenspeicher
system: null
name: Zuverlässigkeitsanfrage bei Sicherheitsbehörden
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
  - gesetz: NDSG
    artikel: § 17
  - gesetz: GewO
    artikel: § 34a Abs. 1a
  - gesetz: WaffG
    artikel: § 5 Abs. 5
  aufbewahrung:
    frist: wie die zugehörige Erlaubnis
    beginn: mit Bestandskraft der Entscheidung
    hinweis: Die Auskunft darf nicht länger vorgehalten werden als die Erlaubnis,
      deren Erteilung sie trägt.
letzte-aktualisierung: '2026-08-10'
tags:
- Zuverlässigkeit
- Verfassungsschutz
- Art. 10 DSGVO
---



# Zuverlässigkeitsanfrage bei Sicherheitsbehörden

## Definition

Auskünfte der Polizei und der Verfassungsschutzbehörde, die im Rahmen einer gesetzlich angeordneten Zuverlässigkeitsprüfung eingeholt werden.

## Felder

- Betroffene Person
- anfragende Stelle und Datum
- angefragte Behörde
- Rechtsgrundlage der Anfrage
- Ergebnis: Bedenken ja oder nein
- übermittelte Erkenntnisse, soweit mitgeteilt
- Verwertung in der Entscheidung

## Hinweise

Angelegt am 2026-08-03 zu `vvt-32-014` (Bewachererlaubnisse) und `vvt-32-017` (Waffen- und Jagdwesen).

**Regelanfrage, kein Ausnahmefall.** § 34a Abs. 1a GewO ordnet für bestimmte Bewachungstätigkeiten die Anfrage bei der Verfassungsschutzbehörde an, § 5 Abs. 5 WaffG für waffenrechtliche Erlaubnisse. Die VVT bezeichnete sie als „ggf." -- gesetzlich vorgesehen ist sie in den genannten Fällen zwingend.

**Nur das Ergebnis, nicht die Erkenntnis.** Die Sicherheitsbehörden teilen der Erlaubnisbehörde regelmäßig nur mit, ob Bedenken bestehen, nicht worin sie bestehen. Das Feld für übermittelte Erkenntnisse ist deshalb im Regelfall leer -- und soll es bleiben. Wird es gefüllt, handelt es sich um Erkenntnisse der Sicherheitsbehörden über eine Person, mit entsprechendem Schutzbedarf.

**Getrennt von der übrigen Erlaubnisakte zu führen.** Wer die Erlaubnis bearbeitet, muss das Ergebnis kennen; wer sie später einsieht, nicht notwendig auch die Anfrage.

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
