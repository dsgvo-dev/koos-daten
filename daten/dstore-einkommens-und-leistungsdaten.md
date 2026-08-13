---
id: dstore-einkommens-und-leistungsdaten
typ: datenspeicher
system: null
name: Einkommens- und Leistungsdaten
datenkategorie: Sozialleistungsdaten
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
  bsi-integritaet: normal
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: BEEG
  - gesetz: SGB
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-10'
tags:
- Einkommen
- Elterngeld
- Mutterschaftsgeld
- Zuschuss
- Einnahmen
---



# Einkommens- und Leistungsdaten

## Definition

Finanz- und Leistungsdaten zur Prüfung von Ansprüchen in sozialrechtlichen Verfahren.

## Felder

- Erwerbseinkommen im Bemessungszeitraum
- voraussichtliches Erwerbseinkommen im Bezugszeitraum
- Mutterschaftsgeld
- Arbeitgeberzuschuss
- sonstige Einnahmen
- Nachweiszeitraum

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- BEEG
- SGB

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Elterngeld, Antrag

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Nur aufgenommen, wenn im Portal explizit als Unterlagen- oder Nachweiskategorie genannt.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Wirtschaftliche Notlage und Sozialleistungsbezug.** Das LfD-Schutzstufenkonzept nennt Sozialdaten, Schulden und Pfändungen ausdrücklich bei Stufe D; § 35 SGB I stellt Sozialdaten zusätzlich unter das Sozialgeheimnis. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Der gemeinsame Nenner ist die Wirkung:** Wird bekannt, dass jemand Leistungen bezieht, Mietschulden hat oder gepfändet wird, beeinträchtigt das die gesellschaftliche Stellung und den Zugang zu Wohnung, Kredit und Arbeit erheblich.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
