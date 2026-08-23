---
id: dstore-nachweis
typ: datenspeicher
system: null
name: Nachweis
zuständige-einheit: oe-amt-33
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
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: NVwVfG
  aufbewahrung:
    frist: Kontextabhängig
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-12'
tags:
- Nachweis
- Beleg
- Dokument
konvertiert-aus: daten1/dtype-nachweis.md
---


## Beschreibung

Allgemeiner Nachweis oder Beleg, der im Rahmen eines Verwaltungsverfahrens eingereicht wird.

## Felder

- Nachweisart
- Aussteller
- Datum
- Inhalt

## Rechtsgrundlage

NVwVfG

## Löschfrist

Kontextabhängig

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-12

**Bleibt bei C.** Nachweisart, Aussteller, Datum, Inhalt.

Ein Behälter ohne festen Inhalt. `pruefung.py` führt diese Gruppe unter den generischen
Speichern (Regel R3: Zuordnung nur mit ausdrücklichem Beleg).

Der Bestand behandelt sie einheitlich auf C: `dstore-bescheid` C, `dstore-bescheinigung` C,
`dstore-verwaltungsakte` C — jeweils geprüft, letzterer mit einer Variante `-vertraulich`
auf D.

**C ist hier keine Verlegenheitslösung, sondern eine Aussage:** Der Behälter allein trägt
keine Einstufung; sie kommt von dem, was hineingelegt wird. Wo Sensibles hineingelegt wird,
steht die benannte Datenart daneben und trägt ihre eigene Stufe.

**`verwendungen: 0` ist hier kein Mangel.** Anders als bei den Hundespeichern aus Los 1
(Amt 32) ist das erwünscht: Ein generischer Behälter *soll* nicht gesetzt werden, wo eine
benannte Datenart passt.

*Durchsicht Los 2 (Amt 33) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los2-amt33.md`.*
