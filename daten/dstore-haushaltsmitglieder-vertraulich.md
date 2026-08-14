---
id: dstore-haushaltsmitglieder-vertraulich
typ: datenspeicher
system: null
name: Haushaltsmitglieder und Haushaltsgröße in vertraulichen Verfahren
datenkategorie: Wohnen & Soziales
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenobjekt
kontext:
  rolle: variante
  variante-von: dstore-haushaltsmitglieder
  bedingung: verfahren-vertraulich
  stufe-basis: C
  stufe-variante: D
  zusatzfeld: Aktenzeichen oder Fallnummer des vertraulichen Verfahrens
  regelquelle: regeln/kontextregeln.yaml
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: SGB I
    artikel: § 35
    titel: Sozialgeheimnis, soweit Sozialdaten betroffen sind
  - gesetz: NDSG
    artikel: § 3
  aufbewahrung:
    frist: nach den Fristen des jeweiligen Fachverfahrens
    beginn: mit Abschluss des Verfahrens
    hinweis: >-
      Die Frist richtet sich nach dem Verfahren, in dem der Speicher gefuehrt wird,
      nicht nach der Datenart.
letzte-aktualisierung: '2026-08-14'
tags:
- Kontextvariante
- Haushalt
- Verfahrenszugehörigkeit
---

# Haushaltsmitglieder und Haushaltsgröße in vertraulichen Verfahren

## Definition

Daten zu den im Haushalt lebenden Personen und ihrer Anzahl in Verfahren, deren
Zugehörigkeit selbst schutzbedürftig ist — Sozialhilfe (SGB XII), Jugendhilfe (SGB VIII),
Asylbewerberleistungen und Leistungen nach dem Infektionsschutzgesetz. Inhaltlich identisch
mit den allgemeinen Haushaltsdaten.

## Felder

- Anzahl Haushaltsmitglieder
- Person im Haushalt
- Verwandtschaftsverhältnis
- Geburtsdatum
- Haushaltszugehörigkeit
- Auszugs-/Einzugsdatum
- Aktenzeichen oder Fallnummer des vertraulichen Verfahrens

## Abgrenzung zu `dstore-haushaltsmitglieder`

**Die Datenart ist dieselbe. Der Unterschied liegt darin, worüber ihre Existenz Auskunft
gibt.**

`dstore-haushaltsmitglieder` steht in Verfahren, deren Zugehörigkeit für die betroffene
Person nicht belastend ist. Dort ist die Haushaltszusammensetzung eine Verwaltungsangabe —
etwa im Wohngeldverfahren.

Dieser Speicher steht in den vertraulichen Verfahren, bei denen **die bloße Tatsache der
Zugehörigkeit schon die schutzbedürftige Information ist**: Wer hier geführt wird, bezieht
Sozialleistungen, erhält Jugendhilfe oder ist von einem Tätigkeitsverbot betroffen. Die
Haushaltsmitglieder sind dann nicht mehr eine neutrale Angabe, sondern die familiäre
Situation einer vulnerablen Person — im Jugendhilfefall sogar Grundlage einer Entscheidung
über ein Kind.

## Hinweise

Angelegt am 2026-08-14 bei der Schutzstufendurchsicht Los 6 (Amt 50). Die Durchsicht hatte
ergeben, dass `dstore-haushaltsmitglieder` ausschließlich in vier vertraulichen Verfahren
geführt wird und dort „familiäre Verhältnisse" einer hilfesuchenden Person trägt. Statt den
allgemeinen Speicher auf D anzuheben (und damit auch jede künftige nicht-vertrauliche
Verwendung zu belegen), wird die Kontextvariante nach dem Muster der Allgemeinplatz-Aufspaltung
geführt.

**Zuordnungsregel für neue Verarbeitungen.** Eine Verarbeitung erhält diese Variante, wenn die
Frage zu bejahen ist: *Wäre es für die betroffene Person nachteilig, wenn bekannt würde, dass
sie in diesem Verfahren geführt wird?* Im Zweifel ist die Variante zu wählen.

## Schutzstufe geprüft 2026-08-14

**Stufe D.** Die Einstufung folgt nicht aus dem Feldinhalt, sondern aus dem
Verfahrenskontext. Das LfD-Schutzstufenkonzept nennt Sozialdaten ausdrücklich als Beispiel
der Stufe D; § 35 SGB I stellt sie unter das Sozialgeheimnis. Bei einer Person, die als
Empfängerin von Sozialleistungen, als Klientin der Jugendhilfe oder als Betroffene eines
Tätigkeitsverbots erkennbar wird, ist die Offenlegung der familiären Verhältnisse erheblich —
unabhängig davon, dass die Datenart selbst nur Namen und Geburtsdaten von
Haushaltsmitgliedern enthält.

## BSI-Vektoren geprüft 2026-08-14

Integrität und Verfügbarkeit entsprechen der Basisvariante (`normal`); sie hängen an der
Datenart, nicht am Verfahren. Die Vertraulichkeit ist `hoch`: Eine Offenlegung träfe die
Kommune als Verantwortliche unmittelbar, weil sie den Kernbereich der Verschwiegenheitspflichten
berührt — § 35 SGB I, § 65 SGB VIII und § 203 StGB für die im Gesundheitsbereich tätigen
Personen.
