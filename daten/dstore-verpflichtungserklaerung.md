---
id: dstore-verpflichtungserklaerung
typ: datenspeicher
system: null
name: Verpflichtungserklärung
zuständige-einheit: oe-amt-47
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
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: AufenthG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Verpflichtung
- Besucher
- Unterhalt
---


# Verpflichtungserklärung

## Definition

Erklärung zur Übernahme von Lebensunterhalts- und Ausreisekosten für Dritte.

## Felder

- Verpflichtungsgeber
- Begünstigte Person
- Bonitätsnachweis
- Zeitraum
- Anlass
- Aktenzeichen

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-10

**C → D.** Die Erklärung nach § 68 AufenthG hat zwei Betroffene. Beim **Verpflichtungsgeber** steht ein Bonitätsnachweis in der Akte, und die Haftung erstreckt sich auf Lebensunterhalt, Krankheits- und Ausreisekosten -- sie kann existenzbedrohend werden und wird nach § 66 Abs. 5 AufenthG vollstreckt. Bei der **begünstigten Person** offenbart die Erklärung den Einreisezweck und eine persönliche Bindung ins Bundesgebiet.

Das Feld „Anlass" nimmt regelmäßig Angaben zu Familienbesuch, Krankheit oder Trauerfall auf.
