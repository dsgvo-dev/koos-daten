---
id: dstore-wildursprungsschein
typ: datenspeicher
system: null
name: Wildursprungsschein
zuständige-einheit: oe-amt-71
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: hoch
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: LMHV
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Wild
- Ursprung
- Schein
---


# Wildursprungsschein

## Definition

Nachweis über Herkunft und Erstuntersuchung von Wild.

## Felder

- Wildart
- Erlegungsdatum
- Erlegungsort
- Erleger/in
- Kennzeichnung
- Bescheinigung

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit hoch.** Der Bestand dient der Gefahrenabwehr. Ist er verfälscht oder im entscheidenden Moment nicht abrufbar, kann die Kommune ihre Schutzaufgabe nicht erfüllen -- mit möglichen Folgen für Leib und Leben.

Er begleitet erlegtes Wild in die Lebensmittelkette und dokumentiert die Untersuchung.

## Schutzstufe geprüft 2026-08-10

**D → B.** **Tiere sind keine betroffenen Personen.** Der gesamte Veterinärbereich stand aus dem Import auf Stufe D, ohne dass eine Angabe über einen Menschen dahinterstünde. Personenbezug besteht allein über die Halterin oder den Betrieb, und dort handelt es sich um gewerbliche Angaben, häufig sogar um eine juristische Person ohne Personenbezug.

Wildart, Erlegungsdatum und -ort. Die Jagdausübung ist eine erlaubte Tätigkeit; der Schein dient der Lebensmittelhygiene.

**Die BSI-Werte bleiben hoch.** Im Seuchenfall entscheidet die Verfügbarkeit dieser Bestände darüber, wie schnell die Kommune eingrenzen kann. Datenschutz und Informationssicherheit fallen hier auseinander -- das ist kein Widerspruch, sondern der Sinn der getrennten Bewertung.
