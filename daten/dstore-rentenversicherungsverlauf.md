---
id: dstore-rentenversicherungsverlauf
typ: datenspeicher
system: null
name: Rentenversicherungsverlauf
datenkategorie: Arbeit & Aufenthalt
zuständige-einheit: oe-amt-47
bpmn:
  typ: datenspeicher
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
  - gesetz: SGB VI
  - gesetz: AufenthG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Rente
- Versicherungsverlauf
- Beiträge
---


# Rentenversicherungsverlauf

## Definition

Versicherungs- und Beitragszeiten in der gesetzlichen Rentenversicherung.

## Felder

- Versicherungsnummer
- Beitragszeiten
- Zeitraum
- Rentenversicherungsträger
- Nachweis
- Person

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-10

**C → D.** **Der Versicherungsverlauf ist eine lückenlose Erwerbsbiografie.** Er weist nicht nur Beitragszeiten aus, sondern in den Lücken auch Arbeitslosigkeit, Krankheit, Reha, Kindererziehung und Pflege. Aus Anrechnungszeiten wegen Krankheit werden Gesundheitsdaten nach Art. 9 DSGVO erkennbar, ohne dass eine Diagnose genannt ist.

Die Datei nennt neben dem SGB VI auch das AufenthG -- der Verlauf dient dann dem Nachweis der Sicherung des Lebensunterhalts im aufenthaltsrechtlichen Verfahren, wo an ihm eine Entscheidung über den Verbleib im Bundesgebiet hängt.
