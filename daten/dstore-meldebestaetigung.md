---
id: dstore-meldebestaetigung
typ: datenspeicher
system: null
name: Meldebestätigung
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: BMG
  aufbewahrung:
    frist: 5 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Meldung
- Bestätigung
- Wohnsitz
konvertiert-aus: daten1/dtype-meldebestaetigung.md
---


## Beschreibung

Amtliche Bestätigung der An- oder Ummeldung eines Wohnsitzes.

## Felder

- Name
- Adresse
- Meldedatum
- Behörde

## Rechtsgrundlage

BMG

## Löschfrist

5 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-10

**B → C.** **Kohärenzkorrektur.** Die Bescheinigung enthält dieselbe Angabe wie `dstore-meldeadresse-wohnsitz` -- den Wohnort einer Person. Dass sie als Dokument und nicht als Registereintrag geführt wird, ändert an der Sensibilität nichts.

Die Anschrift ist die Angabe, an der die praktisch wichtigsten Schutzmaßnahmen des Melderechts hängen: die Auskunftssperre nach § 51 BMG bei Gefahr für Leben, Gesundheit oder Freiheit und der bedingte Sperrvermerk nach § 52 BMG. **Vor jeder Ausstellung ist zu prüfen, ob eine Sperre vorliegt** -- eine Meldebescheinigung, die an die falsche Person gerät, kann eine Schutzsuchende auffindbar machen.
