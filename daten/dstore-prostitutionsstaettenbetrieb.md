---
id: dstore-prostitutionsstaettenbetrieb
typ: datenspeicher
system: null
name: Prostitutionsstättenbetrieb
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: ProstSchG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-12'
tags:
- Prostitutionsstätte
- Betrieb
- Erlaubnis
---



# Prostitutionsstättenbetrieb

## Definition

Betriebsdaten einer erlaubnispflichtigen Prostitutionsstätte.

## Felder

- Betriebsort
- Betreiber/in
- Betriebszeiten
- Nutzungskonzept
- Schutzkonzept
- Erlaubnisstatus

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

**Angehoben von C auf D.** Zwei Gründe, jeder für sich tragend.

**Zuverlässigkeitsprüfung mit Art.-10-Bezug.** Die Erlaubnis nach § 12 ProstSchG ist nach **§ 14 ProstSchG** zu versagen, wenn die erforderliche Zuverlässigkeit fehlt. Nach **§ 15 Abs. 2 ProstSchG** holt die Behörde dafür ein Führungszeugnis für Behörden (§ 30 Abs. 5, §§ 31, 32 Abs. 3 und 4 BZRG) und eine Auskunft der für den Wohnsitz zuständigen Polizeibehörde ein.

**Die Zugehörigkeit zum Speicher offenbart bereits etwas.** Wer als Betreiberin einer Prostitutionsstätte geführt wird, ist damit dem Prostitutionsgewerbe zugeordnet — unabhängig davon, welches Feld gefüllt ist.

**Nicht E.** Die Gefährdung von Leib, Leben oder Freiheit trifft die *in der Prostitution tätigen Personen*; dafür steht `dstore-anmeldebescheinigung-prostschg` bereits auf E. Die Betreiberdaten erreichen diese Schwelle nicht.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
