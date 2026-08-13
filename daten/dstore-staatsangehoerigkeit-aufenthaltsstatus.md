---
id: dstore-staatsangehoerigkeit-aufenthaltsstatus
typ: datenspeicher
system: null
name: Staatsangehörigkeit und Aufenthaltsstatus
datenkategorie: Identitätsdaten
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
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: AufenthG
  - gesetz: PStG
  - gesetz: BEEG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-04'
tags:
- Staatsangehörigkeit
- Aufenthaltstitel
- Ausland
- Ehefähigkeitszeugnis
---



# Staatsangehörigkeit und Aufenthaltsstatus

## Definition

Daten zur Staatsangehörigkeit, ausländerrechtlichen Stellung und grenzüberschreitenden Personenstandsbezügen.

## Felder

- Staatsangehörigkeit
- Nachweis der Staatsangehörigkeit
- Aufenthaltstitel
- Auslandsbezug
- ausländische Urkunde

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- AufenthG
- PStG
- BEEG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Eheschließung, Anmeldung
- Ehefähigkeitszeugnis, Ausstellung
- Beantragung der Befreiung von der Vorlage des Ehefähigkeitszeugnisses
- Sterbefall im Ausland
- Elterngeld, Antrag

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Ausländische Urkunden und Aufenthaltstitel wurden nicht auf Dokumentenebene, sondern als Status- und Nachweiskategorie zusammengeführt.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## Schutzstufe geprüft 2026-08-04

Durchsicht des Katalogs gegen das Schutzstufenkonzept des LfD Niedersachsen,
Maximalprinzip.

**Von C auf D.** Ein aufenthaltsrechtlicher Status entscheidet darüber, ob eine Person im Bundesgebiet bleiben darf. Das Schutzstufenkonzept ordnet der Stufe D Daten zu, deren Missbrauch die Existenz beeinträchtigen kann -- bei einer Aufenthaltsbeendigung ist das unmittelbar der Fall.

Hinzu kommt die faktische Wirkung: Der Aufenthaltsstatus wird gesellschaftlich als Merkmal der Herkunft gelesen, auch wenn er rechtlich keine Angabe über die ethnische Herkunft nach Art. 9 Abs. 1 DSGVO ist.

Der Speicher verbindet Staatsangehörigkeit, ausländerrechtliche Stellung und Auslandsbezug. Er wird auch in `vvt-47-003` (AsylbLG-Leistungen) geführt und offenbart dort zusätzlich den Leistungsbezug.

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

