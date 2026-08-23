---
id: dstore-finanzielle-leistungsfaehigkeit
typ: datenspeicher
system: null
name: Nachweis der finanziellen Leistungsfähigkeit
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
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c
  - gesetz: NDSG
    artikel: § 3
  - gesetz: VO (EG) 1071/2009
    artikel: Art. 7
  - gesetz: GüKG
    artikel: § 3
  - gesetz: GBZugV
    artikel: § 2
  aufbewahrung:
    frist: wie die zugehörige Erlaubnis, längstens 10 Jahre
    beginn: nach Erlöschen der Erlaubnis
    hinweis: Die Leistungsfähigkeit ist nach Art. 7 Abs. 1 VO (EG) 1071/2009 jährlich
      nachzuweisen; ältere Nachweise verlieren ihre Aussagekraft und sind zu löschen.
letzte-aktualisierung: '2026-08-10'
tags:
- Güterkraftverkehr
- finanzielle Leistungsfähigkeit
- Berufszugang
---



# Nachweis der finanziellen Leistungsfähigkeit

## Definition

Nachweise über Eigenkapital, Reserven oder eine Bürgschaft, mit denen ein Unternehmen die finanzielle Leistungsfähigkeit für den Zugang zum Beruf des Kraftverkehrsunternehmers belegt.

## Felder

- Unternehmen und vertretungsberechtigte Person
- Zahl der genutzten Fahrzeuge
- erforderlicher Betrag (9.000 EUR für das erste, 5.000 EUR für jedes weitere Fahrzeug)
- Eigenkapital und Reserven aus dem geprüften Jahresabschluss
- ausstellende Person der Eigenkapitalbescheinigung
- alternativ: Bankbürgschaft oder Versicherung nach Art. 7 Abs. 2
- Datum und Gültigkeit des Nachweises
- Feststellung bei Nichterfüllung mit Begründung

## Hinweise

Angelegt am 2026-08-03 zu `vvt-32-009` (Güterkraftverkehr), nach Prüfung des Verordnungstextes.

**Was Art. 7 VO (EG) 1071/2009 verlangt.** Das Unternehmen weist anhand der von einem Rechnungsprüfer geprüften Jahresabschlüsse nach, dass es jedes Jahr über Eigenkapital und Reserven von mindestens 9.000 EUR für das erste und 5.000 EUR für jedes weitere genutzte Fahrzeug verfügt (Abs. 1). Alternativ kann die Behörde eine Bankbürgschaft oder eine Versicherung als selbstschuldnerische Bürgschaft gelten lassen (Abs. 2). § 2 GBZugV lässt für Deutschland die Eigenkapitalbescheinigung eines Wirtschaftsprüfers, vereidigten Buchprüfers, Steuerberaters, Steuerbevollmächtigten, Rechtsanwalts oder Kreditinstituts genügen; ist das Unternehmen nach § 316 Abs. 1 HGB prüfungspflichtig, muss die Bescheinigung vom Abschlussprüfer stammen.

**Personenbezug besteht bei Einzelunternehmen und Personengesellschaften unmittelbar.** Dort ist das Eigenkapital des Unternehmens zugleich das Vermögen einer natürlichen Person.

**Stufe D nach dem Maximalprinzip.** Der positive Nachweis allein wäre nach dem LfD-Konzept Stufe C -- wirtschaftliche Verhältnisse. Der Speicher führt aber auch die **Feststellung bei Nichterfüllung**, und die stützt sich auf dieselben Tatsachen wie eine Gewerbeuntersagung: Zahlungsrückstände, Vollstreckungsmaßnahmen, Insolvenzbezug. Das Konzept nennt Schulden ausdrücklich als Stufe-D-Beispiel. Maßgeblich ist die sensibelste Angabe, die anfallen kann.

Dieselbe Begründung wie bei `dstore-gewerbeuntersagung`.

**Jährlicher Nachweis, jährliche Löschung.** Da die Leistungsfähigkeit fortlaufend bestehen muss, entsteht jedes Jahr ein neuer Nachweis. Ältere Jahresabschlüsse verlieren ihre Aussagekraft für die laufende Erlaubnis und sind nicht aufzubewahren, nur weil sie einmal vorlagen.

**Auch bei der Personenbeförderung einschlägig.** § 2 PBZugV verlangt für Taxi- und Mietwagenkonzessionen dieselbe Prüfung. In `vvt-32-010` ist sie bei den Datenkategorien nicht genannt; ob sie dort geführt wird, ist zu klären.

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

**Bleibt bei D.** Die Einstufung wurde am 2026-08-04 bei der Anlage beziehungsweise
Überarbeitung dieses Speichers ausführlich begründet -- siehe die Hinweise oben. Der
Durchgang vom 2026-08-10 hat sie bestätigt und trägt hier nur den Prüfvermerk nach, der bisher
fehlte.

*Der Vermerk ist kein Formalismus: Ohne ihn zählte der Speicher als ungeprüft, und der
Rückstand wies 129 statt der tatsächlich offenen 115 Speicher aus -- allesamt auf Stufe C.*
