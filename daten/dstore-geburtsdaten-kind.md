---
id: dstore-geburtsdaten-kind
typ: datenspeicher
system: null
name: Geburtsdaten eines Kindes
datenkategorie: Personenstandsdaten
zuständige-einheit: oe-amt-31
bpmn:
  typ: nachricht
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
  - gesetz: PStG
  - gesetz: PStV
  - gesetz: BEEG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-10'
tags:
- Kind
- Geburt
- Geburtsurkunde
- Hausgeburt
- Geburtsanzeige
---



# Geburtsdaten eines Kindes

## Definition

Daten zur Geburt eines Kindes für Registereinträge, Urkunden und familienbezogene Leistungsansprüche.

## Felder

- Vorname des Kindes
- Familienname des Kindes
- Geburtsdatum
- Geburtszeit
- Geburtsort
- Geburtsnachweis

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: nachricht

## Rechtsgrundlagen

- PStG
- PStV
- BEEG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Geburt, Anzeige
- Hausgeburt Anzeige
- Urkunde, Geburtsurkunde/Geburtenregister, Beantragung
- Elterngeld, Antrag

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Kindbezogene Daten wurden von Eltern- und Registerbezug getrennt, um Wiederverwendung zu erleichtern.

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

## Schutzstufe geprüft 2026-08-10

**D → C.** **Personenstandsdaten sind nicht als Gruppe hochsensibel.** Die Durchsicht hat sie einzeln geprüft, statt sie pauschal auf D zu belassen. Auf D bleiben die Speicher, die Abstammung, Sorgerechtsentscheidungen oder die Religionszugehörigkeit führen -- `dstore-personenstand`, `dstore-elternbezug-abstammung`, `dstore-sorgerechtsnachweis`, `dstore-sorgerechtserklaerung` und `dstore-geburtsanzeige-unterlagenpaket`.

Name, Geburtsdatum, Geburtszeit und Geburtsort eines Kindes. Die Angaben werden in der Geburtsurkunde beurkundet und sind gegenüber jedem vorzulegen, der einen Nachweis verlangt.
