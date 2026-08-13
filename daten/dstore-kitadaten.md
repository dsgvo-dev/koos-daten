---
id: dstore-kitadaten
typ: datenspeicher
system: null
name: Kitadaten
datenkategorie: Soziales & Jugend
zuständige-einheit: oe-amt-51
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
  - gesetz: SGB VIII
  - gesetz: NKiTaG
  aufbewahrung:
    frist: 5 Jahre nach Austritt
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Kita
- Betreuung
- Kind
konvertiert-aus: daten1/dtype-kitadaten.md
---



## Beschreibung

Daten zur Kita-Anmeldung und Betreuungsvertrag.

## Felder

- Kind
- Sorgeberechtigte
- Betreuungsumfang
- Betreuungsbeginn
- Einrichtung

## Rechtsgrundlage

SGB VIII, NKiTaG

## Löschfrist

5 Jahre nach Austritt

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

## Schutzstufe geprüft 2026-08-10

**Bleibt bei C.** Wie `dstore-kita-anmeldedaten`; hier zusätzlich der Betreuungsvertrag nach dem NKiTaG.

**Anmerkung zur Modellpflege:** Die beiden Speicher überschneiden sich so weit, dass unklar bleibt, wann welcher gemeint ist -- `kita-anmeldedaten` führt vvt-51-005 und vvt-51-004, `kitadaten` vvt-51-015 und vvt-51-004. Eine Zusammenführung wäre zu prüfen; sie ist keine Frage der Schutzstufe und wird deshalb hier nur vermerkt.
