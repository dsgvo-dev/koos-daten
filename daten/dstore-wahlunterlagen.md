---
id: dstore-wahlunterlagen
typ: datenspeicher
system: null
name: Wahlunterlagen
zuständige-einheit: oe-amt-10
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: NKomVG
  - gesetz: BWG
  - gesetz: NKWG
  aufbewahrung:
    frist: 6 Monate nach Wahl
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-04'
tags:
- Wahl
- Wahlunterlagen
- Demokratie
konvertiert-aus: daten1/dtype-wahlunterlagen.md
---



## Beschreibung

Unterlagen zu Wahlen: Wählerverzeichnis, Wahlschein, Briefwahlunterlagen.

## Felder

- Wähler
- Wahlbezirk
- Wahlschein
- Stimmzettel
- Briefwahlunterlagen

## Rechtsgrundlage

NKomVG, BWG, NKWG

## Löschfrist

6 Monate nach Wahl

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

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

## Schutzstufe geprüft 2026-08-14

**C bestätigt.** Das Wahlgeheimnis (Art. 38 GG) macht Wahlunterlagen besonders schützenswert
— der Frontmatter-Wert `schutzbedarf: hoch` trägt das. Kein D: Der Stimmzettel ist anonym,
der Wahlschein identifiziert die Teilnahmeart, nicht die Stimmabgabe; die politische Meinung
(Art. 9 DSGVO) wird durch das Datenmodell nicht offenbart. Das Wahlgeheimnis wird
verfahrensseitig gewahrt, nicht durch die Datenart.

Geprüft im Rahmen der Schutzstufendurchsicht Los 4 (Amt 10). Vorschlag:
`_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-14-los4-amt10.md`.

