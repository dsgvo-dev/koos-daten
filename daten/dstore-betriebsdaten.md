---
id: dstore-betriebsdaten
typ: datenspeicher
system: null
name: Betriebsdaten
datenkategorie: Gewerbe & Wirtschaft
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
  - gesetz: HGB
  - gesetz: GewO
  aufbewahrung:
    frist: 10 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-12'
tags:
- Betrieb
- Unternehmen
- Firma
konvertiert-aus: daten1/dtype-betriebsdaten.md
---


## Beschreibung

Stammdaten eines Unternehmens oder Betriebs.

## Felder

- Firmenname
- Rechtsform
- Handelsregisternummer
- Geschäftsführer
- USt-ID

## Rechtsgrundlage

HGB, GewO

## Löschfrist

10 Jahre

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

**Herabgestuft von C auf B.** Der gesamte Inhalt ist von Gesetzes wegen öffentlich einsehbar:

- **§ 9 Abs. 1 HGB** — die Einsicht in das Handelsregister und die zu ihm eingereichten Dokumente ist jedem zu Informationszwecken gestattet.
- **§ 79 Abs. 1 BGB** — die Einsicht in das Vereinsregister und die von dem Verein zum Register eingereichten Schriftstücke ist jedem gestattet.

Personenbezug hat allein der gesetzliche Vertreter, und zwar in seiner Funktion, nicht als Privatperson. Eine unbefugte Offenbarung nimmt niemandem etwas, was nicht ohnehin abrufbar wäre.

**Warum B und nicht A.** Stufe A setzt voraus, dass die betroffene Person die Daten *selbst frei zugänglich gemacht* hat — Telefonverzeichnis, eigene Webseite. Eine Registereintragung ist Pflicht, keine freiwillige Veröffentlichung, und der kommunale Auszug liegt nicht offen. B trifft es: nicht frei zugänglich, Missbrauch ohne besondere Beeinträchtigung.

Der Inhalt — Firmenname, Rechtsform, Handelsregisternummer, Geschäftsführer, USt-ID — ist eine Teilmenge von `dstore-unternehmens-und-registerdaten`. Die beiden Speicher überschneiden sich weitgehend; eine Zusammenlegung wäre zu erwägen, gehört aber nicht in eine Schutzstufendurchsicht.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
