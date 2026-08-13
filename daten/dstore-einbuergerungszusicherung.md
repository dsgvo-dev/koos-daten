---
id: dstore-einbuergerungszusicherung
typ: datenspeicher
system: null
name: Einbürgerungszusicherung
datenkategorie: Migration & Einbürgerung
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
  bsi-integritaet: normal
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: StAG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-04'
tags:
- Einbürgerung
- Zusicherung
---



# Einbürgerungszusicherung

## Definition

Zusicherungs- und Verfahrensdaten einer beabsichtigten Einbürgerung.

## Felder

- Aktenzeichen
- Zusicherungsdatum
- Voraussetzungen
- Aufgabe bisheriger Staatsangehörigkeit
- Person
- Gültigkeit

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## Schutzstufe geprüft 2026-08-04

Durchsicht des Katalogs gegen das Schutzstufenkonzept des LfD Niedersachsen,
Maximalprinzip.

**Von C auf D.** Ein aufenthaltsrechtlicher Status entscheidet darüber, ob eine Person im Bundesgebiet bleiben darf. Das Schutzstufenkonzept ordnet der Stufe D Daten zu, deren Missbrauch die Existenz beeinträchtigen kann -- bei einer Aufenthaltsbeendigung ist das unmittelbar der Fall.

Hinzu kommt die faktische Wirkung: Der Aufenthaltsstatus wird gesellschaftlich als Merkmal der Herkunft gelesen, auch wenn er rechtlich keine Angabe über die ethnische Herkunft nach Art. 9 Abs. 1 DSGVO ist.

Die Zusicherung setzt voraus, dass die bisherige Staatsangehörigkeit aufgegeben wird. Zwischen Zusicherung und Einbürgerung kann Staatenlosigkeit entstehen -- ein existenzieller Zwischenzustand.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `normal`** · **Verfügbarkeit: `hoch`**

**Über `normal` gesetzt: Verfügbarkeit `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Integrität bleibt bei `normal`**, geprüft anhand der Fragen des Durchgangs vom 2026-08-04:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

