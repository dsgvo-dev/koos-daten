---
id: dstore-leistungsbezug-sozialleistung
typ: datenspeicher
system: null
name: Leistungsbezug Sozialleistung
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: sehr hoch
  bsi-verfuegbarkeit: sehr hoch
  bsi-schutzbedarf: sehr hoch
  rechtsgrundlagen:
  - gesetz: SGB II
  - gesetz: SGB XII
  - gesetz: WoGG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-10'
tags:
- Sozialleistung
- Leistungsbezug
- Bescheid
---



# Leistungsbezug Sozialleistung

## Definition

Bewilligungs- und Nachweisdaten zu laufenden Sozialleistungen.

## Felder

- Leistungsart
- bewilligende Stelle
- Aktenzeichen
- Bewilligungszeitraum
- Zahlbetrag
- Bescheid

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- SGB II
- SGB XII
- WoGG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Bildung und Teilhabe beantragen
- Förderung für Bildung und Teilhabe von Kindern und jungen Erwachsenen beantragen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `sehr hoch`** · **Verfügbarkeit: `sehr hoch`**

**Über `normal` gesetzt: Integrität `sehr hoch` und Verfügbarkeit `sehr hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Wirtschaftliche Notlage und Sozialleistungsbezug.** Das LfD-Schutzstufenkonzept nennt Sozialdaten, Schulden und Pfändungen ausdrücklich bei Stufe D; § 35 SGB I stellt Sozialdaten zusätzlich unter das Sozialgeheimnis. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Der gemeinsame Nenner ist die Wirkung:** Wird bekannt, dass jemand Leistungen bezieht, Mietschulden hat oder gepfändet wird, beeinträchtigt das die gesellschaftliche Stellung und den Zugang zu Wohnung, Kredit und Arbeit erheblich.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
