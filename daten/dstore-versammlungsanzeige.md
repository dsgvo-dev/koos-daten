---
id: dstore-versammlungsanzeige
typ: datenspeicher
system: null
name: Versammlungsanzeige und Auflagen
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
    artikel: Art. 9 Abs. 2 lit. g
  - gesetz: NDSG
    artikel: § 17
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c
  - gesetz: NVersG
    artikel: § 5
  - gesetz: GG
    artikel: Art. 8
  aufbewahrung:
    frist: 3 Jahre
    beginn: nach der Versammlung
    hinweis: Rechtsbehelfsfristen und mögliche Amtshaftungsansprüche; Festlegung des
      Trägers. Bei Versammlungen, die ohne Beanstandung verlaufen sind, ist eine kürzere
      Frist zu erwägen.
letzte-aktualisierung: '2026-08-10'
tags:
- Versammlungsrecht
- Art. 8 GG
- Art. 9 DSGVO
---



# Versammlungsanzeige und Auflagen

## Definition

Anzeige einer Versammlung nach § 5 NVersG einschließlich Thema, Route und angeordneter Beschränkungen.

## Felder

- Anzeigende und versammlungsleitende Person
- Kontaktdaten
- Thema der Versammlung
- Ort, Route und Zeit
- erwartete Teilnehmerzahl
- Kooperationsgespräch
- angeordnete Beschränkungen mit Begründung
- Rechtsbehelfe

## Hinweise

Angelegt am 2026-08-03 zu `vvt-32-018` (Versammlungsrechtliche Verfahren).

**Das Thema der Versammlung offenbart die politische Meinung.** Wer eine Versammlung zu einem bestimmten Anliegen anmeldet und leitet, gibt damit eine Überzeugung nach Art. 9 Abs. 1 DSGVO preis. Bei religiös oder weltanschaulich geprägten Versammlungen tritt das entsprechende Merkmal hinzu.

**Die Grundrechtslage verschärft den Schutzbedarf.** Die anzeigende Person muss ihren Namen nennen, um von Art. 8 GG Gebrauch zu machen. Wer eine Versammlung anmelden will, kann das nicht anonym tun -- die Preisgabe ist Voraussetzung der Grundrechtsausübung, nicht deren Folge.

Daraus folgt praktisch: enger Zugriffskreis, keine Führung in allgemein zugänglichen Vorgangslisten, keine Übermittlung ohne ausdrückliche Rechtsgrundlage.

VERWORFEN bei der Zuordnung: `dstore-ausnahmegenehmigung-schwerverkehr` -- über einen gemeinsamen Prozess aus dem Schwertransportverfahren hereingetragen.

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

**Bleibt bei D.** **Familiäre, aufenthaltsrechtliche und weltanschauliche Verhältnisse.** Anders als bei den am selben Tag herabgestuften Personenstandsspeichern trägt dieser Bestand eine Angabe, die für sich genommen belastend ist -- eine Sorgerechtsentscheidung, die Abstammung, die Religionszugehörigkeit, den Aufenthaltsstatus oder die Ausübung eines Grundrechts. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
