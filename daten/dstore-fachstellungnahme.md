---
id: dstore-fachstellungnahme
typ: datenspeicher
system: null
name: Fachstellungnahme
datenkategorie: Verwaltungsformular
zuständige-einheit: oe-amt-63
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: NBauO
    artikel: §63 Abs. 2
    titel: Beteiligung von Behörden
  - gesetz: VwVfG
    artikel: §73
    titel: Anhörungsverfahren
  aufbewahrung:
    frist: 10 Jahre nach Abschluss des Verfahrens
    beginn: nach Bestandskraft des Bescheids
    hinweis: Bestandteil der Bauakte; Grundlage für Auflagen im Bescheid
letzte-aktualisierung: '2026-08-04'
---


# Fachstellungnahme

## Definition

Schriftliche Äußerung einer beteiligten Fachbehörde oder Fachstelle zu einem Bauvorhaben.
Sie ist ein zentrales intermediäres Datenobjekt im Baugenehmigungsverfahren: Jede Fachstelle,
deren Aufgabenbereich berührt ist, gibt eine Stellungnahme ab, die in die Entscheidung einfließt.

## Typische Aussteller und Inhalte

- **Brandschutz** (oe-amt-37): Beurteilung der Brandschutzanforderungen, Auflagenvorschläge
- **Tiefbau / Erschließung** (oe-amt-66): Stellungnahme zur Erschließung, Entwässerung
- **Stadtplanung** (oe-amt-61): Übereinstimmung mit Bebauungsplan, Befreiungsbedarf
- **Denkmalschutz** (Landesdenkmalamt): Bei denkmalgeschützten Gebäuden oder Umgebung
- **Umwelt** (oe-amt-60): Naturschutz, Baumschutz, Bodenschutz

## Hinweise

Die Frist für Stellungnahmen beträgt in der Regel einen Monat. Schweigen gilt nicht als
Zustimmung; bei Fristablauf ohne Rückmeldung kann die Bauaufsicht weitermachen (§ 63 NBauO).
Widersprüche zwischen Fachstellungnahmen sind von der Bauaufsicht zu koordinieren.

## Schutzstufe geprüft 2026-08-04

Geprüft im Zuge der Auflösung von `vvt-61-001` und `vvt-61-002`: Alle Speicher mit
Freitextfeldern wurden gegen das Schutzstufenkonzept des LfD Niedersachsen gehalten.
Maßstab ist das Maximalprinzip -- die sensibelste Angabe, die anfallen **kann**.

Die entscheidende Frage lautet: **Schreibt die betroffene Person selbst hinein, oder
formuliert eine Fachstelle?** Ist der Text von außen frei bestimmbar, ist mit Angaben nach
Art. 9 Abs. 1 DSGVO zu rechnen. Formuliert eine Behörde sachbezogen, ist er es nicht.

**Bleibt bei B.** Die Stellungnahme wird von einer beteiligten Fachbehörde formuliert und betrifft ein Bauvorhaben, nicht eine Person. Der Text ist fachlich gebunden und nicht von außen frei bestimmbar -- das unterscheidet ihn von der Bürgerstellungnahme nach § 3 Abs. 2 BauGB, für die `dstore-stellungnahme-planverfahren` mit Stufe D angelegt wurde.

Der Speicher wird derzeit in keiner Verarbeitungstätigkeit verwendet. Vor einer künftigen Verwendung ist zu prüfen, ob er noch gebraucht wird.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*
