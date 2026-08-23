---
id: dstore-aufwandsentschaedigung-ehrenamt
typ: datenspeicher
system: null
name: Aufwandsentschädigung und Reisekosten im Ehrenamt
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: EStG
    artikel: § 3 Nr. 26a
  - gesetz: NKomHKVO
  - gesetz: AO
    artikel: § 147
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Ablauf des Kalenderjahres der Auszahlung
    hinweis: § 147 Abs. 3 AO für Buchungsbelege.
letzte-aktualisierung: '2026-08-04'
tags:
- Ehrenamt
- Aufwandsentschädigung
- Gremien
---



# Aufwandsentschädigung und Reisekosten im Ehrenamt

## Definition

Abrechnung von Reisekosten und Aufwandsentschädigungen für ehrenamtlich tätige Personen in Beiräten, Ausschüssen und Gremien.

## Felder

- Ehrenamtlich tätige Person
- Gremium oder Anlass
- Sitzungs- oder Reisedatum
- Strecke und Verkehrsmittel
- Betrag der Entschädigung
- Bankverbindung
- steuerliche Behandlung

## Hinweise

Angelegt am 2026-08-03 zu `vvt-50-008` (Abrechnung Behindertenbeirat).

**Zwei Namensfallen führten hierher.** Die VVT nannte „Abrechnungsdaten" -- `dstore-abrechnungsdaten` führt aber Gehalts- und Lohnabrechnungen von Beschäftigten. Und `dstore-reisekosten-aufenthaltsverfahren` betrifft ausländerrechtliche Verfahren. Beide heißen fast wie das Gesuchte und meinen etwas anderes.

Verwendbar für alle Gremien und Beiräte, nicht nur den Behindertenbeirat.

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

## Schutzstufe geprüft 2026-08-14

**Bleibt bei C.** Betrag, Bankverbindung, Gremium und steuerliche Behandlung offenbaren
wirtschaftliche Verhältnisse (C-Kriterium). Eine Anhebung auf D scheidet aus: Der
Behindertenbeirat offenbart kein Gesundheitsdatum — dem Beirat gehören nach dem Vermerk in
`vvt-50-008` auch Angehörige und Fachleute an, sodass die Mitgliedschaft für sich genommen
keinen Schluss auf eine Behinderung zulässt.


