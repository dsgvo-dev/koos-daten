---
id: dstore-gewerbedaten
typ: datenspeicher
system: null
name: Gewerbedaten
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: GewO
  - gesetz: GewAnzV
  aufbewahrung:
    frist: 10 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-12'
tags:
- Gewerbe
- Gewerbeanmeldung
- Betrieb
konvertiert-aus: daten1/dtype-gewerbedaten.md
---


## Beschreibung

Daten zur An-, Um- oder Abmeldung eines Gewerbes.

## Felder

- Gewerbetreibender
- Betriebsart
- Betriebsanschrift
- Anmeldedatum
- Gewerbenummer

## Rechtsgrundlage

GewO, GewAnzV

## Löschfrist

10 Jahre

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

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** Das Gewerberegister ist **kein** öffentliches Register — anders als Handels- und Vereinsregister. Nach § 14 GewO erteilt die Behörde Dritten Auskunft, wenn ein berechtigtes Interesse glaubhaft gemacht wird; die einfache Auskunft beschränkt sich auf Gewerbename, Anschrift und angezeigte Tätigkeit.

Damit scheidet Stufe A aus — frei zugänglich sind die Daten nicht. Ihre Offenbarung beeinträchtigt aber weder die gesellschaftliche Stellung noch die wirtschaftlichen Verhältnisse: Ein angemeldetes Gewerbe wird nach außen betrieben; Firmenschild, Briefkopf und Impressum nennen dieselben Angaben.

**Zum Verwendungskontext.** Der Speicher steht auch in `vvt-32-012` (Reisegewerbekarten, Art. 10 DSGVO). Nach R6 Schritt 2 gilt im Zweifel der sensible Kontext. Hier greift das nicht: Die sensible Angabe — die Zuverlässigkeitsprüfung nach § 57 Abs. 1 GewO — liegt in einem **eigenen** Speicher, `dstore-reisegewerbekarte`, der am 2026-08-12 auf D angehoben wurde. Die effektive Stufe der Verarbeitung bleibt dadurch unverändert.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
