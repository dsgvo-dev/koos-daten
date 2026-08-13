---
id: dstore-namensaenderungsnachweis
typ: datenspeicher
system: null
name: Namensänderungsnachweis
datenkategorie: Identitätsdaten
zuständige-einheit: oe-amt-33
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
  - gesetz: NamÄndG
  - gesetz: BGB
  - gesetz: PStG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-12'
tags:
- Namensänderung
- Heirat
- Urkunde
---


# Namensänderungsnachweis

## Definition

Nachweise über eine Änderung des Familien- oder Vornamens.

## Felder

- bisheriger Name
- neuer Name
- Grund der Änderung
- Änderungsdatum
- Nachweisart
- ausstellende Stelle

## Klassifizierung

- Schutzstufe: D
- Schutzbedarf: hoch
- Vertraulichkeit: streng vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- NamÄndG
- BGB
- PStG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Personalausweis – Neuausstellung wegen Namensänderung bei Heirat
- Personalausweis – Neuausstellung wegen Namensänderung aus sonstigen Gründen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Der Name wirkt lebenslang und in alle Register hinein.

## Schutzstufe geprüft 2026-08-12

**Angehoben von C auf D.**

**Das gefährliche Datum ist nicht der Name, sondern die Verknüpfung.** Wer den bisherigen und
den neuen Namen nebeneinander sieht, kann eine Person, die ihren Namen gewechselt hat, wieder
auffinden. Eine öffentlich-rechtliche Namensänderung setzt nach § 3 Abs. 1 NamÄndG einen
wichtigen Grund voraus; zu den anerkannten Gründen zählt der Schutz vor Nachstellung.

Der Bestand stuft die Nachbardaten bereits so ein: `dstore-namensaenderungsgrund` steht auf
**D**, `dstore-frueherer-name-personenstandsaenderung` auf **E** (§ 13 SBGG,
Offenbarungsverbot, bußgeldbewehrt). Ein Speicher, der beide Namen führt, kann nicht darunter
liegen.

**Nicht E.** Die Fälle, in denen die Offenbarung Leib, Leben oder Freiheit bedroht, sind über
`auskunftssperre-melderegister` und `schutzbeduerftigkeitskennzeichen` (beide E) abgedeckt.
`vvt-31-001` führt beide und steht deshalb bereits auf effektiv E.

*Durchsicht Los 2 (Amt 33) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los2-amt33.md`.*
