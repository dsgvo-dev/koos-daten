---
id: dstore-hundehaltung
typ: datenspeicher
system: null
name: Hundehaltung
zuständige-einheit: oe-amt-32
bpmn:
  typ: nachricht
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
  - gesetz: NHundG
  - gesetz: kommunale Satzung
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-12'
tags:
- Hund
- Haltung
- Anmeldung
---



# Hundehaltung

## Definition

Grunddaten zur Haltung eines Hundes im Gemeindegebiet.

## Felder

- Halterin oder Halter
- Beginn Hundehaltung
- Hundename
- Rasse
- Geburtsdatum Hund
- Haltungsanschrift

## Klassifizierung

- Schutzstufe: B
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: nachricht

## Rechtsgrundlagen

- NHundG
- kommunale Satzung

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Hundehaltung Anmeldung
- Einen Hund anmelden
- Hundehaltung Abmeldung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `hoch`** · **Verfügbarkeit: `normal`**

**Über `normal` gesetzt: Integrität `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Verfügbarkeit bleibt bei `normal`**, geprüft anhand der Fragen des Durchgangs vom 2026-08-04:

1. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** Halterin oder Halter, Beginn der Haltung, Hundename, Rasse, Geburtsdatum des Hundes, Haltungsanschrift.

Die Haltung eines Hundes ist ein nach außen sichtbarer Alltagsvorgang. Für die *gewöhnliche* Hundehaltung trägt keine dieser Datenarten eine Beeinträchtigung der betroffenen Person.

**Abgrenzung.** `dstore-erlaubnis-gefaehrlicher-hund` und `dstore-maulkorb-leinenanordnung` bleiben bei C. Dort belegt der Eintrag einen ordnungsrechtlichen Vorgang gegen die Halterin — die Feststellung der Gefährlichkeit nach § 7 NHundG. Der Unterschied ist nicht der Hund, sondern der Verwaltungsakt.

**Lücke im Verzeichnis.** `verwendungen: 0`, obwohl die Kommune diese Daten führt. Sachlich gehört der Speicher zur Hundesteuer (`vvt-22-004`) und zur Haltungsüberwachung (`vvt-71-002`). Als eigener Auftrag vorgemerkt.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
