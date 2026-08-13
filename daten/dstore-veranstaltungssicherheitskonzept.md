---
id: dstore-veranstaltungssicherheitskonzept
typ: datenspeicher
system: null
name: Veranstaltungssicherheitskonzept
datenkategorie: Veranstaltungen & Sicherheit
zuständige-einheit: oe-amt-32
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
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: NVersG
  - gesetz: StVO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-12'
tags:
- Veranstaltung
- Sicherheit
- Konzept
---



# Veranstaltungssicherheitskonzept

## Definition

Sicherheits- und Ordnungskonzept für Veranstaltungen mit Publikumsverkehr.

## Felder

- Veranstaltung
- Ort
- Besucherzahl
- Sicherheitsmaßnahmen
- Rettungswege
- Verantwortliche Person

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

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

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** Veranstaltung, Ort, Besucherzahl, Sicherheitsmaßnahmen, Rettungswege, verantwortliche Person.

Personenbezug besteht allein über die verantwortliche Person, und zwar in ihrer Funktion. Der Inhalt beschreibt eine Veranstaltung, keinen Menschen.

**`bsi-verfuegbarkeit` bleibt hoch.** Das ist kein Widerspruch: Für die betroffene Person ist das Konzept harmlos, für die Kommune im Ereignisfall unverzichtbar. Die beiden Maßstäbe messen Verschiedenes — der Datenschutz den Schaden für die Person, der BSI-Grundschutz den Schaden für die Institution.

**Lücke im Verzeichnis.** `verwendungen: 0`. Der Speicher gehört sachlich zu `vvt-10-012` (Veranstaltungsmanagement) oder zu einer Verarbeitung des Amtes 32. Als eigener Auftrag vorgemerkt.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
