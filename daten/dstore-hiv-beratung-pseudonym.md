---
id: dstore-hiv-beratung-pseudonym
typ: datenspeicher
system: null
name: Pseudonyme HIV-Beratung und -Testung
datenkategorie: Gesundheit & Soziales
zuständige-einheit: oe-amt-53
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: E
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: sehr hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: sehr hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. h und lit. i
  - gesetz: NDSG
    artikel: § 17
  - gesetz: IfSG
    artikel: § 19
  aufbewahrung:
    frist: bis zum Abschluss der Beratung, längstens sechs Monate
    beginn: nach Ausgabe des Testergebnisses
    hinweis: Festlegung des Trägers. Die Nummer ist zu vernichten, sobald das Ergebnis
      übergeben ist; danach besteht kein Zweck mehr für die Zuordnung.
letzte-aktualisierung: '2026-08-10'
tags:
- IfSG
- HIV
- Art. 9 DSGVO
- Schutzstufe E
---



# Pseudonyme HIV-Beratung und -Testung

## Definition

Unter einer Nummer geführte Angaben zu Beratung und Testung auf HIV und andere sexuell übertragbare Krankheiten nach § 19 IfSG.

## Felder

- Vorgangsnummer
- Testart und Testdatum
- Testergebnis
- Beratungsinhalt
- Ausgabedatum des Ergebnisses
- Vernichtungsvermerk der Nummer

## Hinweise

Angelegt am 2026-08-03 zu `vvt-53-010` (AIDS-Beratung).

**Pseudonym, nicht anonym.** Die VVT bezeichnete die Daten als „anonymisiert (Nummernverfahren)". Anonyme Daten fielen nach Erwägungsgrund 26 DSGVO nicht unter die Verordnung -- dann wäre der Verzeichniseintrag entbehrlich. Tatsächlich erlaubt die Nummer die Zuordnung des Ergebnisses zur ratsuchenden Person; das ist Pseudonymisierung nach Art. 4 Nr. 5 DSGVO und damit personenbezogen. Die Datei zitiert Art. 9 Abs. 2 selbst und setzt Gesundheitsdaten also voraus.

**Schutzstufe E.** Ein HIV-Status kann bei Offenbarung Existenz, Gesundheit und persönliche Sicherheit gefährden.

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

**Bleibt bei E.** Ein HIV-Testergebnis ist ein Gesundheitsdatum nach Art. 9 DSGVO und zugleich eine Angabe, deren Offenlegung zu Ausgrenzung, Verlust des Arbeitsplatzes und Gewalt führen kann.

**§ 19 IfSG ordnet die anonyme Beratung an**, und die Pseudonymisierung ist hier nicht Schutzmaßnahme, sondern Bedingung dafür, dass Menschen den Test überhaupt in Anspruch nehmen. Fällt sie weg, fällt die Prävention weg. Der Vernichtungsvermerk der Vorgangsnummer ist deshalb die entscheidende Maßnahme; er ist nachzuhalten.

**Korrektur vom 2026-08-03 bleibt gültig:** Die zugehörige Verarbeitung behauptete Anonymität, obwohl pseudonymisiert wird. Der Unterschied ist rechtlich erheblich -- pseudonyme Daten sind personenbezogen.
