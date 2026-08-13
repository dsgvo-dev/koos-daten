---
id: dstore-lebenspartnerschaftsurkunde-nachweis
typ: datenspeicher
system: null
name: Lebenspartnerschaftsurkunde als Nachweis
datenkategorie: Personenstandsdaten
zuständige-einheit: oe-amt-31
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
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: PStG
  - gesetz: LPartG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-04'
tags:
- Lebenspartnerschaft
- Urkunde
- Nachweis
---


# Lebenspartnerschaftsurkunde als Nachweis

## Definition

Urkundendaten zu einer eingetragenen Lebenspartnerschaft als Nachweis eines Personenstands.

## Felder

- Partner 1
- Partner 2
- Begründungsdatum
- Begründungsort
- Urkundennummer
- Ausstellungsdatum

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- PStG
- LPartG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Lebenspartnerschaftsurkunde beantragen

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## Schutzstufe geprüft 2026-08-04

Geprüft im Zuge der Auflösung von `vvt-61-001` und `vvt-61-002`: Alle Speicher mit
Freitextfeldern wurden gegen das Schutzstufenkonzept des LfD Niedersachsen gehalten.
Maßstab ist das Maximalprinzip -- die sensibelste Angabe, die anfallen **kann**.

Die entscheidende Frage lautet: **Schreibt die betroffene Person selbst hinein, oder
formuliert eine Fachstelle?** Ist der Text von außen frei bestimmbar, ist mit Angaben nach
Art. 9 Abs. 1 DSGVO zu rechnen. Formuliert eine Behörde sachbezogen, ist er es nicht.

**Von C auf D -- ein Befund, der nicht am Freitext hängt.**

Eine eingetragene Lebenspartnerschaft konnte nach dem LPartG **ausschließlich zwischen zwei Personen gleichen Geschlechts** begründet werden. Seit dem 1. Oktober 2017 werden keine neuen mehr eingetragen; bestehende bestehen fort. Der Nachweis einer Lebenspartnerschaft offenbart damit zwangsläufig die sexuelle Orientierung der betroffenen Person -- ein Datum nach **Art. 9 Abs. 1 DSGVO**.

Der Unterschied zur Heirats- oder Eheurkunde ist wesentlich: Seit der Öffnung der Ehe lässt eine Eheurkunde diesen Schluss nicht zu, eine Lebenspartnerschaftsurkunde immer. `dstore-heiratsurkunde` und `dstore-eheurkunde-nachweis` bleiben deshalb unverändert.

Der EuGH hat den Begriff der sensiblen Daten zum Sexualleben weit gefasst und auf Angaben erstreckt, aus denen sich solche Informationen mittels Ableitung ergeben (Urt. v. 05.06.2023, C-204/21, und Urt. v. 02.12.2025, C-492/23). Genau das liegt hier vor.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*
