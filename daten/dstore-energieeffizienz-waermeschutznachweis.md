---
id: dstore-energieeffizienz-waermeschutznachweis
typ: datenspeicher
system: null
name: Energieeffizienz- und Wärmeschutznachweis
datenkategorie: Bauen & Energie
zuständige-einheit: oe-amt-63
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
  - gesetz: GEG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Energie
- Wärmeschutz
- Nachweis
---


# Energieeffizienz- und Wärmeschutznachweis

## Definition

Nachweise zu energetischen Anforderungen und Wärmeschutz eines Gebäudes.

## Felder

- Gebäudeart
- U-Werte
- Primärenergiebedarf
- Nachweisart
- Aussteller/in
- Gültigkeit

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei B.** **Sach- und Objektdaten mit mittelbarem Personenbezug.** Gegenstand ist ein Grundstück, ein Bauteil oder ein Behälter; die Person kommt als Eigentümerin, Pflichtige oder Planende hinzu. Aus der Datenart lässt sich nichts über Gesundheit, wirtschaftliche Lage oder Verhalten ableiten. Ein Teil der Angaben ist ohnehin öffentlich zugänglich -- das Baulastenverzeichnis nach § 81 Abs. 3 NBauO wird auf berechtigtes Interesse hin eingesehen, Katasterdaten nach § 12 NVermG.

*Sammelvermerk der Durchsicht vom 2026-08-10.*
