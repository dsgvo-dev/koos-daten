---
id: dstore-spende-zuwendung
typ: datenspeicher
system: null
name: Spende und Zuwendung
datenkategorie: Finanzen & Zahlung
zuständige-einheit: oe-amt-10
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: NKomVG
    artikel: § 111 Abs. 8
  - gesetz: EStDV
    artikel: § 50
  - gesetz: AO
    artikel: § 147
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Ablauf des Kalenderjahres der Zuwendung
    hinweis: § 147 Abs. 3 AO für Buchungsbelege und Zuwendungsbestätigungen.
letzte-aktualisierung: '2026-08-04'
tags:
- Spende
- Zuwendung
- NKomVG
---



# Spende und Zuwendung

## Definition

Angaben zu einer Spende oder Zuwendung an die Kommune einschließlich Zweckbindung und Zuwendungsbestätigung.

## Felder

- Zuwendende Person oder Organisation
- Spendenbetrag
- Datum und Zahlungsart
- Zweckbindung
- Sachspende mit Bezeichnung und Wert
- ausgestellte Zuwendungsbestätigung
- Annahmebeschluss nach § 111 Abs. 8 NKomVG

## Hinweise

Angelegt am 2026-08-03 zu `vvt-10-017` (Spenden).

**Die Annahme ist nach § 111 Abs. 8 NKomVG beschlusspflichtig.** Der Beschluss und die Zweckbindung gehören zur Datenart, weil sie über die Zulässigkeit der Annahme entscheiden -- eine Zuwendung mit unzulässiger Zweckbindung darf nicht angenommen werden. Ohne diese Felder ist die Prüfung nicht nachvollziehbar.

Die Zuwendungsbestätigung nach § 50 EStDV ist über `dstore-bescheinigung` erfasst; hier steht nur der Vermerk, dass und wann sie ausgestellt wurde.

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

## Schutzstufe geprüft 2026-08-14

**C bestätigt.** Der Spendenbetrag und die Zuwendungsbestätigung nach § 50 EStDV berühren
die wirtschaftlichen Verhältnisse des Spenders. Rechtsgrundlage berichtigt: § 97 NKomVG
(alte Nummerierung) → § 111 Abs. 8 NKomVG (aktuelle Nummerierung nach der
Kommunalrechtsreform) — konsistent mit `vvt-10-017`.

Geprüft im Rahmen der Schutzstufendurchsicht Los 4 (Amt 10). Vorschlag:
`_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-14-los4-amt10.md`.

