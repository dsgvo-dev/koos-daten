---
id: dstore-bildungs-und-teilhabebedarf
typ: datenspeicher
system: null
name: Bildungs- und Teilhabebedarf
zuständige-einheit: oe-amt-51
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: normal
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: SGB II
  - gesetz: WoGG
  - gesetz: BKGG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-10'
tags:
- Bildung
- Teilhabe
- Förderbedarf
---


# Bildungs- und Teilhabebedarf

## Definition

Antrags- und Bedarfsdaten zu Leistungen des Bildungs- und Teilhabepakets.

## Felder

- Leistungsbereich
- Kind oder junger Mensch
- Bedarfszeitraum
- beantragte Leistung
- Einrichtung
- Nachweis

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- SGB II
- WoGG
- BKGG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Bildung und Teilhabe beantragen
- Förderung für Bildung und Teilhabe von Kindern und jungen Erwachsenen beantragen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-10

**C → D.** Die Leistung wird nur gewährt, wenn die Familie hilfebedürftig ist -- § 28 SGB II, § 34 SGB XII und § 6b BKGG knüpfen sie an den Bezug von Bürgergeld, Sozialhilfe, Wohngeld oder Kinderzuschlag. **Die Datenart offenbart deshalb aus sich heraus den Leistungsbezug einer Familie**, auch wenn kein einziger Betrag darin steht. Das LfD-Schutzstufenkonzept nennt Sozialdaten ausdrücklich als Fall der Stufe D; § 35 SGB I stellt sie unter das Sozialgeheimnis.

Hinzu kommt, wen es trifft: Kinder, deren Bedürftigkeit in Schule, Verein und Mensa für Mitschüler sichtbar werden kann. Genau davor schützt die Einstufung.

Der Sammelspeicher des Pakets; er führt Leistungsbereich und Bedarfszeitraum zusammen.
