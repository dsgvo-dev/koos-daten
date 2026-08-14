---
id: dstore-kfz-daten
typ: datenspeicher
system: null
name: KFZ-Daten
datenkategorie: Ordnung & Sicherheit
zuständige-einheit: oe-amt-34
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: FZV
  - gesetz: StVG
  aufbewahrung:
    frist: 7–10 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-04'
tags:
- KFZ
- Zulassung
- Kennzeichen
- Fahrzeug
konvertiert-aus: daten1/dtype-kfz-daten.md
---



## Beschreibung

Daten zur Kfz-Zulassung: Fahrzeughalter, Kennzeichen, Fahrzeugdaten.

## Felder

- Kennzeichen
- Fahrzeughalter
- FIN
- Fahrzeugtyp
- Zulassungsdatum
- HU-Datum

## Rechtsgrundlage

FZV, StVG

## Löschfrist

7–10 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

*(Bitte ergänzen)*

## Schutzstufe geprüft 2026-08-14

**C bestätigt.** Die KFZ-Zulassungsdaten (Kennzeichen, Fahrzeughalter, FIN, Fahrzeugtyp) enthalten Standard-Personendaten (Halter = Name) ohne Art. 9-Bezug. Die Fahrzeug-Sachdaten sind nicht personenbezogen. Keine sensiblen Merkmale — C ist angemessen.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `hoch`** · **Verfügbarkeit: `hoch`**

**Über `normal` gesetzt: Integrität `hoch` und Verfügbarkeit `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

