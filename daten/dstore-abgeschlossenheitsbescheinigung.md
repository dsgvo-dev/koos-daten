---
id: dstore-abgeschlossenheitsbescheinigung
typ: datenspeicher
system: null
name: Abgeschlossenheitsbescheinigung
datenkategorie: Bauen & Eigentum
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
  - gesetz: WEG
  - gesetz: NBauO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Abgeschlossenheit
- WEG
- Bescheinigung
---


# Abgeschlossenheitsbescheinigung

## Definition

Daten zu einer Bescheinigung über die Abgeschlossenheit von Wohnungen oder Einheiten.

## Felder

- Objekt
- Einheiten
- Planbezug
- Antragsteller/in
- Bescheiddatum
- Aktenzeichen

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Sie ist Voraussetzung für die Begründung von Wohnungseigentum und geht ins Grundbuch ein.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei B.** **Sach- und Objektdaten mit mittelbarem Personenbezug.** Gegenstand ist ein Grundstück, ein Bauteil oder ein Behälter; die Person kommt als Eigentümerin, Pflichtige oder Planende hinzu. Aus der Datenart lässt sich nichts über Gesundheit, wirtschaftliche Lage oder Verhalten ableiten. Ein Teil der Angaben ist ohnehin öffentlich zugänglich -- das Baulastenverzeichnis nach § 81 Abs. 3 NBauO wird auf berechtigtes Interesse hin eingesehen, Katasterdaten nach § 12 NVermG.

*Sammelvermerk der Durchsicht vom 2026-08-10.*
