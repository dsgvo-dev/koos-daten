---
id: dstore-bussgeldakte
typ: datenspeicher
system: null
name: Bußgeldakte
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
  - gesetz: OWiG
  aufbewahrung:
    frist: 3–5 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Bußgeld
- Ordnungswidrigkeit
- Verkehr
konvertiert-aus: daten1/dtype-bussgeldakte.md
---



## Beschreibung

Akte zu einem Ordnungswidrigkeitenverfahren.

## Felder

- Aktenzeichen
- Betroffener
- Tatvorwurf
- Tatzeit
- Tatort
- Bußgeldbescheid

## Rechtsgrundlage

OWiG

## Löschfrist

3–5 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-10

**C → D.** Die Akte führt Tatvorwurf, Tatzeit und Tatort. **Der Speicher ist nicht auf eine Deliktsart beschränkt** -- er wird in vier Verarbeitungen geführt, vom ruhenden Verkehr bis zum Umweltrecht, und kann ebenso Verstöße gegen das Schwarzarbeitsbekämpfungsgesetz, das IfSG oder das Gewerberecht aufnehmen. Nach dem Maximalprinzip ist die sensibelste Angabe maßgeblich, die anfallen kann.

Das LfD-Schutzstufenkonzept nennt Straffälligkeit bei Stufe D. Eine Ordnungswidrigkeit ist keine Straftat im Sinne des Art. 10 DSGVO, aber die soziale Wirkung einer Ahndung -- gegenüber Arbeitgeber, Erlaubnisbehörde oder Nachbarschaft -- ist dieselbe. Für das Verfahren gilt zudem der Zweite Teil des NDSG.
