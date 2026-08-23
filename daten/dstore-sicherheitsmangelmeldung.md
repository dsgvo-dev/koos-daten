---
id: dstore-sicherheitsmangelmeldung
typ: datenspeicher
system: null
name: Sicherheitsmangelmeldung
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: NPOG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-12'
tags:
- Sicherheitsmangel
- Meldung
- Gefahr
---



# Sicherheitsmangelmeldung

## Definition

Hinweis- oder Meldedaten zu Sicherheitsmängeln im öffentlichen Raum.

## Felder

- Ort
- Mangelbeschreibung
- Gefahrenstufe
- Meldedatum
- Meldende Person
- Bearbeitungsstatus

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

**Bleibt bei C.** Die Mangelbeschreibung ist Freitext und von außen frei bestimmbar; sie kann benennen, wer den Mangel verursacht hat. Zugleich ist die meldende Person schutzwürdig: Wird bekannt, wer eine Meldung abgesetzt hat, entsteht ein Nachbarschaftskonflikt.

**Nicht D.** Anders als `dstore-beschwerde-anregungsdaten`, das im Freitext regelmäßig Angaben nach Art. 9 DSGVO trägt, betrifft dieser Speicher Zustände im öffentlichen Raum — Schlaglöcher, defekte Beleuchtung, Verkehrsgefahren. Die Existenz eines Eintrags sagt über die betroffene Person nichts Nachteiliges aus.

**Breitenwirkung geprüft.** Sieben Verwendungen in fünf Ämtern. Eine Anhebung hätte `vvt-10-023`, `vvt-15-005`, `vvt-10-028`, `vvt-66-003`, `vvt-34-005`, `vvt-34-004` und `vvt-10-010` mitgezogen — genau die Entwertung, gegen die sich ADR 010 richtet.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
