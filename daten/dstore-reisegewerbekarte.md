---
id: dstore-reisegewerbekarte
typ: datenspeicher
system: null
name: Reisegewerbekarte
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
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
  - gesetz: GewO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-12'
tags:
- Reisegewerbe
- Karte
- Erlaubnis
---



# Reisegewerbekarte

## Definition

Erlaubnisdaten im Zusammenhang mit einem Reisegewerbe.

## Felder

- Karteninhaber/in
- Tätigkeitsumfang
- Geltungsbereich
- Gültigkeit
- Zuverlässigkeitsprüfung
- Gebühren

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

**Angehoben von C auf D.** Der Speicher führt das Feld „Zuverlässigkeitsprüfung".

Nach **§ 57 Abs. 1 GewO** ist die Reisegewerbekarte zu versagen, „wenn Tatsachen die Annahme rechtfertigen, daß der Antragsteller die für die beabsichtigte Tätigkeit erforderliche Zuverlässigkeit nicht besitzt". Die Prüfung stützt sich auf Führungszeugnis und Gewerbezentralregister. Der Speicher trägt damit Angaben zu strafrechtlichen Verurteilungen im Sinne des **Art. 10 DSGVO**.

Die verwendende Verarbeitung bestätigt das: `vvt-32-012` (Reisegewerbekarten) nennt in ihrer Rechtsgrundlage ausdrücklich „Art. 10 DSGVO i. V. m. § 57 GewO (Versagung)".

Das LfD-Schutzstufenkonzept nennt **Straffälligkeit** als Beispiel der Stufe D.

**Abgrenzung zu `dstore-gewerbedaten`.** Die Gewerbestammdaten stehen in einem eigenen Speicher und bleiben bei B. Die sensible Angabe liegt hier, nicht dort. Genau dafür ist die Trennung da.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
