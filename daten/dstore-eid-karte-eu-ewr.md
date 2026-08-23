---
id: dstore-eid-karte-eu-ewr
typ: datenspeicher
system: null
name: eID-Karte EU/EWR
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: eIDKG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-12'
tags:
- eID
- EU
- EWR
- Karte
---



# eID-Karte EU/EWR

## Definition

Daten zur eID-Karte für Unionsbürgerinnen und Unionsbürger sowie EWR-Angehörige.

## Felder

- Kartenart
- Inhaber/in
- Gültigkeit
- Ausstellende Behörde
- Sperrkennwort
- Seriennummer

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

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

**Bleibt bei C.** Kartenart, Inhaber/in, Gültigkeit, ausstellende Behörde, **Sperrkennwort**,
Seriennummer.

**Ausweisdaten ermöglichen Identitätsmissbrauch**, und der trifft die wirtschaftlichen
Verhältnisse — das Kriterium der Stufe C. `dstore-ausweisdokument` steht bereits geprüft auf C.

**Nicht D.** Identitätsmissbrauch bedroht nicht die Existenz im Sinne des LfD-Konzepts, das
dort Gesundheitsdaten, Sozialdaten, Schulden und Straffälligkeit nennt.

**Das Sperrkennwort gibt den Ausschlag gegen eine Herabstufung.** Es ist ein
Zugangsgeheimnis, kein beschreibendes Datum. Ein Speicher, der ein Geheimnis führt, gehört
nicht unter C.

**Rechtsgrundlage berichtigt (2026-08-12).** Die Datei nannte das PAuswG. Das trifft nicht
zu: Die eID-Karte für Unionsbürgerinnen und Unionsbürger sowie Angehörige des EWR beruht auf
dem **eIDKG** — dem Gesetz über eine Karte für Unionsbürger und Angehörige des Europäischen
Wirtschaftsraums mit Funktion zum elektronischen Identitätsnachweis, in Kraft seit dem
1. November 2019. Das PAuswG gilt für deutsche Staatsangehörige; für sie führt der Bestand
`dstore-ausweisdokument`.

*Durchsicht Los 2 (Amt 33) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los2-amt33.md`.*
