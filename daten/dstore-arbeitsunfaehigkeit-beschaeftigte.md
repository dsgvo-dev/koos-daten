---
id: dstore-arbeitsunfaehigkeit-beschaeftigte
bereich: intern
typ: datenspeicher
system: null
name: Arbeitsunfähigkeit der Beschäftigten
zuständige-einheit: oe-amt-11
personenbezug: ja
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. b und lit. c
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. b
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  - gesetz: NBG
    artikel: § 88, § 94 Abs. 2
  - gesetz: EFZG
    artikel: § 5
  - gesetz: SGB IV
    artikel: § 109
  - gesetz: SGB IX
    artikel: § 167 Abs. 2
  - gesetz: SGB V
    artikel: § 44 (teilweise Arbeitsunfähigkeit ab 01.01.2028)
  aufbewahrung:
    frist: 5 Jahre
    beginn: nach Ablauf des Jahres, in dem die Bearbeitung des einzelnen Vorgangs abgeschlossen wurde
    hinweis: 'Frist aus § 94 Abs. 2 Satz 1 NBG für Unterlagen über Erkrankungen; gilt nach § 12 Abs. 1 NDSG auch für Tarifbeschäftigte. Unterlagen, aus denen die Art einer Erkrankung ersichtlich ist, sind nach § 94 Abs. 2 Satz 2 NBG unverzüglich zurückzugeben oder zu vernichten, sobald sie nicht mehr benötigt werden.'
letzte-aktualisierung: '2026-10-05'
tags:
- Personal
- Arbeitsunfähigkeit
- eAU
- Gesundheitsdaten
- Beschäftigtendaten
---

# Arbeitsunfähigkeit der Beschäftigten

## Definition

Zeiten der Arbeitsunfähigkeit und der teilweisen Arbeitsunfähigkeit von Beschäftigten der Kommune (Beamtinnen und Beamte, Tarifbeschäftigte, Auszubildende), wie sie die Personalstelle aus dem eAU-Abruf nach § 109 SGB IV oder aus vorgelegten Bescheinigungen führt. Dient der Entgeltfortzahlung, der Abwesenheitsverwaltung und der Ermittlung der Sechs-Wochen-Schwelle für das betriebliche Eingliederungsmanagement.

## Felder

- Personalnummer und Name
- Organisationseinheit
- Beginn der Arbeitsunfähigkeit
- voraussichtliches und tatsächliches Ende der Arbeitsunfähigkeit
- Datum der ärztlichen Feststellung
- Erst- oder Folgebescheinigung
- Kennzeichen Arbeitsunfall oder sonstiger Unfall
- teilweise Arbeitsunfähigkeit mit Stufe (25 / 50 / 75 %; Feststellung ab 01.01.2028)
- Nachweisart (eAU-Abruf, vorgelegte Bescheinigung)

Keine Diagnose. Der Arbeitgeber erhält beim eAU-Abruf keine Diagnose; vorgelegte Bescheinigungen mit Diagnoseangabe fallen unter § 94 Abs. 2 Satz 2 NBG.

## Hinweise

**Anlass.** Angelegt am 2026-10-05. Die Arbeitsunfähigkeit der Beschäftigten war bis dahin in `dstore-arbeitsunfaehigkeit-krankheit` geführt, einem aus Serviceportal-Texten abgeleiteten Datentyp für Bürgerverfahren (zuständig oe-amt-53, Rechtsgrundlagen SGB V und BEEG, Feld „Diagnosehinweis“, Aufbewahrung „prozessabhängig“). Für Beschäftigte gelten eine andere Rechtsgrundlage, ein anderer Zugriffskreis und eine feste Löschfrist.

**Schutzstufe D.** Schon die Tatsache der Arbeitsunfähigkeit ist ein Gesundheitsdatum nach Art. 9 Abs. 1 DSGVO; das LfD-Konzept ordnet Gesundheitsdaten der Stufe D zu.

**Vertraulichkeitsklasse vertraulich.** Der Zugriffskreis ist begrenzt (Personalstelle, BEM-Beauftragte für die Schwellenmeldung), aber nicht auf eine Stelle beschränkt: Fachvorgesetzte erfahren den Abwesenheitszeitraum. Streng vertraulich ist die BEM-Akte (`dstore-bem-verfahrensdaten`).

**BSI-Vektoren.** Vertraulichkeit hoch: Bekanntwerden verletzt Art. 9 DSGVO, mit Bußgeld- und Vertrauensfolgen. Integrität normal: Die Daten sind bei der Krankenkasse erneut abrufbar; eine Verfälschung wirkt sich auf den einzelnen Vorgang aus. Verfügbarkeit normal: Ein Ausfall verzögert Entgeltabrechnung und Fristberechnung, verhindert sie nicht.

**Abgrenzung zu ähnlichen Speichern:**
- `dstore-arbeitsunfaehigkeit-krankheit`: Bürgerverfahren (oe-amt-53), Nachweise mit möglichem Diagnosehinweis; nicht für Beschäftigte.
- `dstore-urlaubs-und-abwesenheitsdaten`: Urlaub und sonstige Abwesenheiten; Krankheit dort nur als Abwesenheitsart ohne AU-Angaben, Frist drei Jahre (Erholungsurlaub).
- `dstore-bem-verfahrensdaten`: Inhalte des BEM-Verfahrens; erhält aus diesem Speicher nur die Meldung, dass die Sechs-Wochen-Schwelle erreicht ist.
