---
id: dstore-baulastenauszug
typ: datenspeicher
system: null
name: Baulastenauszug
datenkategorie: Bauen & Grundstück
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
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: NBauO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Baulast
- Auszug
- Grundstück
---


# Baulastenauszug

## Definition

Auszugsdaten aus dem Baulastenverzeichnis.

## Felder

- Grundstück
- Baulastart
- Eintragungsdatum
- Inhalt
- Aktenzeichen
- Auskunftsempfänger/in

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Baulasten wirken gegenüber jedem Rechtsnachfolger. Ein unvollständiger Auszug führt zu Bauvorhaben, die sich nachträglich als unzulässig erweisen.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei B.** **Sach- und Objektdaten mit mittelbarem Personenbezug.** Gegenstand ist ein Grundstück, ein Bauteil oder ein Behälter; die Person kommt als Eigentümerin, Pflichtige oder Planende hinzu. Aus der Datenart lässt sich nichts über Gesundheit, wirtschaftliche Lage oder Verhalten ableiten. Ein Teil der Angaben ist ohnehin öffentlich zugänglich -- das Baulastenverzeichnis nach § 81 Abs. 3 NBauO wird auf berechtigtes Interesse hin eingesehen, Katasterdaten nach § 12 NVermG.

*Sammelvermerk der Durchsicht vom 2026-08-10.*
