---
id: dstore-schulbesuch-ausbildungsstatus
typ: datenspeicher
system: null
name: Schulbesuch und Ausbildungsstatus
datenkategorie: Bildung & Betreuung
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenobjekt
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
  - gesetz: SGB II
  - gesetz: BKGG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-10'
tags:
- Schule
- Ausbildung
- Teilnahme
---


# Schulbesuch und Ausbildungsstatus

## Definition

Daten zum Schulbesuch oder Ausbildungsstatus von Kindern, Jugendlichen oder jungen Erwachsenen.

## Felder

- Schule oder Ausbildungseinrichtung
- Klassenstufe
- Ausbildungsstatus
- Schulbescheinigung
- Beginn
- Ende

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- SGB II
- BKGG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Bildung und Teilhabe beantragen
- Förderung für Bildung bei jungen Erwachsenen

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

**Bleibt bei C.** Die Statusangabe selbst ist eine Schulbescheinigung: Einrichtung, Klassenstufe, Zeitraum. Das trägt keine Stufe D, auch wenn der Speicher in sieben Verarbeitungen geführt wird, von denen einige -- etwa das Bildungs- und Teilhabepaket -- der Bedürftigkeitsprüfung dienen. **Die Bedürftigkeit folgt dort aus dem Leistungsspeicher, nicht aus der Schulbescheinigung.**

Anzuheben wäre der Speicher, sobald er die Schulform in einer Weise ausweist, die einen sonderpädagogischen Förderbedarf erkennen lässt -- das wäre ein Gesundheitsdatum nach Art. 9 DSGVO. Das Feld „Schulform" in `dstore-schulbedarf-lernamaterial` ist daraufhin im Auge zu behalten.
