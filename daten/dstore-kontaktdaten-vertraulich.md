---
id: dstore-kontaktdaten-vertraulich
typ: datenspeicher
system: null
name: Telefonnummer, Mobilnummer und E-Mail-Adresse von Personen in Verfahren, deren Zugehörigke
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
kontext:
  rolle: variante
  variante-von: dstore-kontaktdaten
  bedingung: verfahren-vertraulich
  stufe-basis: B
  stufe-variante: D
  zusatzfeld: Vermerk ueber Kontaktbeschraenkungen
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
letzte-aktualisierung: '2026-08-10'
tags:
- Kontextvariante
- Allgemeinplatz
- Gewaltschutz
---

# Telefonnummer, Mobilnummer und E-Mail-Adresse von Personen in Verfahren, deren Zugehörigke

## Definition

Telefonnummer, Mobilnummer und E-Mail-Adresse von Personen in Verfahren, deren Zugehörigkeit selbst schutzbedürftig ist.

## Felder

- Telefonnummer
- Mobilnummer
- E-Mail-Adresse
- bevorzugter Kontaktweg
- Vermerk über Kontaktbeschränkungen (etwa: keine Nachricht auf der Mailbox, kein Anruf zu bestimmten Zeiten, kein Postversand an die Wohnanschrift)

## Abgrenzung zu `dstore-kontaktdaten`

**Die Datenart ist dieselbe. Der Unterschied liegt darin, worüber ihre Existenz Auskunft gibt.**

`dstore-kontaktdaten` steht in Verfahren, deren Zugehörigkeit für die betroffene Person nicht belastend
ist -- eine Gewerbeanmeldung, ein Bauantrag, eine Ummeldung, eine Wahlbenachrichtigung. Dort
ist der Name ein Name.

Dieser Speicher steht in den 19 Verfahren, bei denen **die bloße Tatsache der Zugehörigkeit
schon die schutzbedürftige Information ist**: Sozialhilfe, Jugendhilfe, Sozialpsychiatrie,
Aufenthaltsrecht, Bußgeldverfahren, Vollstreckung, Gesundheitsamt, Bewerbungsverfahren,
Beratungsangebote. Wer hier geführt wird, ist bedürftig, krank, verdächtigt, verschuldet oder
sucht Hilfe -- und das ergibt sich bereits aus der Zuordnung, ohne dass ein Inhalt gelesen
werden müsste.

**Das Feld für Kontaktbeschränkungen ist der eigentliche Zugewinn dieser Variante.** In der Sozialpsychiatrie, im Kindeswohlschutz und in der Gleichstellungsberatung kann ein Rückruf zur falschen Zeit oder eine Nachricht auf einem mitgehörten Anschluss eine Person gefährden. Die allgemeine Variante sieht dieses Feld nicht vor -- sie braucht es nicht, und ihr Fehlen war bisher ein blinder Fleck.

## Hinweise

Angelegt am 2026-08-10 bei der Aufspaltung der Allgemeinplätze. Die Durchsicht hatte gezeigt,
dass `dstore-kontaktdaten` über 24 Organisationseinheiten streut und deshalb keine einheitliche
Schutzstufe tragen kann: Eine niedrige Stufe unterschätzt die vertraulichen Verfahren, eine
hohe Stufe belegt die Routineverfahren mit Maßnahmen, die sie nicht brauchen.

**Zuordnungsregel für neue Verarbeitungen.** Eine Verarbeitung erhält diese Variante, wenn die
Frage zu bejahen ist: *Wäre es für die betroffene Person nachteilig, wenn bekannt würde, dass
sie in diesem Verfahren geführt wird?* Im Zweifel ist die Variante zu wählen -- die
Herabstufung eines Einzelfalls ist leichter zu begründen als die nachträgliche Anhebung.

## Schutzstufe geprüft 2026-08-10

**Stufe D.** Die Einstufung folgt nicht aus dem Feldinhalt, sondern aus dem Verfahrenskontext.
Das LfD-Schutzstufenkonzept knüpft an die Frage, ob die Offenlegung die gesellschaftliche
Stellung oder die wirtschaftlichen Verhältnisse erheblich beeinträchtigen kann. Bei einer
Person, die als Empfängerin von Sozialleistungen, als Betroffene eines Bußgeldverfahrens oder
als Klientin der Sozialpsychiatrie erkennbar wird, ist das zu bejahen -- unabhängig davon,
dass die Datenart selbst nur einen Namen oder eine Telefonnummer enthält.

## BSI-Vektoren geprüft 2026-08-10

Integrität und Verfügbarkeit entsprechen der Basisvariante; sie hängen an der Datenart, nicht
am Verfahren. Die Vertraulichkeit ist hoch: Eine Offenlegung träfe die Kommune als
Verantwortliche unmittelbar, weil sie den Kernbereich der Verschwiegenheitspflichten berührt
-- § 35 SGB I, § 65 SGB VIII und § 203 StGB für die im Gesundheitsbereich tätigen Personen.
