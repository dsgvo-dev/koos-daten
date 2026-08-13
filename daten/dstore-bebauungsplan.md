---
id: dstore-bebauungsplan
typ: datenspeicher
system: null
name: Bebauungsplan / Flächennutzungsplan
datenkategorie: Bescheid / Nachweis
zuständige-einheit: oe-amt-61
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: A
  schutzbedarf: normal
  vertraulichkeitsklasse: öffentlich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: BauGB
    artikel: §8
    titel: Bebauungsplan
  - gesetz: BauGB
    artikel: §5
    titel: Flächennutzungsplan
  - gesetz: NBauO
    artikel: §63
    titel: Prüfung planungsrechtlicher Zulässigkeit
  aufbewahrung:
    frist: dauerhaft (öffentliche Satzung)
    beginn: null
    hinweis: Bebauungspläne sind öffentliche Satzungen; kein Ablaufdatum
letzte-aktualisierung: '2026-08-10'
---


# Bebauungsplan / Flächennutzungsplan

## Definition

Verbindliche städtebauliche Planungsdokumente der Gemeinde. Der Bebauungsplan setzt
die Art und das Maß der baulichen Nutzung eines Gebiets fest (§ 8 BauGB); der
Flächennutzungsplan ist das übergeordnete, nicht unmittelbar verbindliche Dokument.

Im BPMN-Sinne sind sie **Data Stores**: Sie werden von mehreren Prozessen referenziert
(Baugenehmigungsverfahren, Bauvoranfrage, Befreiungsantrag), ohne selbst Teil des
Prozessflusses zu sein. Zuständig für ihre Pflege ist das Stadtplanungsamt (oe-amt-61),
nicht das Bauamt.

## Verwendung im Baugenehmigungsverfahren

Das Bauamt prüft bei jedem Bauantrag die planungsrechtliche Zulässigkeit anhand des
geltenden Bebauungsplans. Liegt kein Bebauungsplan vor, richtet sich die Zulässigkeit
nach §34 oder §35 BauGB (Innen-/Außenbereich).

## Hinweise

Bebauungspläne sind öffentlich einsehbar (§ 10 Abs. 3 BauGB). Änderungen erfordern
ein formelles Planänderungsverfahren mit Öffentlichkeitsbeteiligung.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-10

**Bleibt bei A.** **Der einzige Speicher der Stufe A -- zu Recht.** Bauleitpläne sind Ortsrecht. Sie werden nach § 10 Abs. 3 BauGB ortsüblich bekannt gemacht und sind jedermann zugänglich; § 3 BauGB ordnet die Auslegung sogar ausdrücklich an. Eine Angabe, deren Veröffentlichung das Gesetz verlangt, kann nicht schutzbedürftig sein.

**Die Abgrenzung ist die Stellungnahme.** Was Bürgerinnen und Bürger im Beteiligungsverfahren vortragen, ist `dstore-stellungnahme-planverfahren` und steht auf Stufe D. Der Plan ist öffentlich, der Weg dorthin nicht.
