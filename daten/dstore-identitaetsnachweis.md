---
id: dstore-identitaetsnachweis
typ: datenspeicher
system: null
name: Identitätsnachweis
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: PAuswG
  - gesetz: PassG
  - gesetz: DSGVO
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-12'
tags:
- Personalausweis
- Reisepass
- eID
- Passersatz
- Legitimation
---



# Identitätsnachweis

## Definition

Daten aus amtlichen Identitätsdokumenten zur Legitimation der antragstellenden, vertretenen oder erklärenden Person.

## Felder

- Dokumentart
- Dokumentnummer
- Vorname
- Familienname
- Gültigkeitsdatum
- ausstellende Behörde
- eID-Nutzung

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: datenobjekt

## Rechtsgrundlagen

- PAuswG
- PassG
- DSGVO

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Urkunde, Geburtsurkunde/Geburtenregister, Beantragung
- Geburt, Anzeige
- Dokumente und Kopien: Beglaubigung
- Vorläufige Dokumente, Beantragung
- Personalausweis Beantragung
- Reisepass Beantragung
- Elterngeld, Antrag

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Der Typ deckt sowohl Ausweisdaten als auch Passdaten ab; biometrische Elemente sind separat ausgelagert.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** Der Speicher wird in so vielen Verfahren geführt, dass ein Ausfall nicht ein Verfahren verzögert, sondern den Publikumsverkehr insgesamt zum Erliegen bringt. Das ist der Maßstab des BSI: erhebliche Beeinträchtigung der Aufgabenerfüllung.

Ohne Identitätsprüfung darf am Schalter nichts ausgegeben werden.

## Schutzstufe geprüft 2026-08-12

**Bleibt bei C.** Dokumentart, Dokumentnummer, Vor- und Familienname, Gültigkeitsdatum,
ausstellende Behörde, eID-Nutzung.

**Ausweisdaten ermöglichen Identitätsmissbrauch**, und der trifft die wirtschaftlichen
Verhältnisse — das Kriterium der Stufe C. `dstore-ausweisdokument` steht bereits geprüft auf C.

**Nicht D.** Identitätsmissbrauch bedroht nicht die Existenz im Sinne des LfD-Konzepts, das
dort Gesundheitsdaten, Sozialdaten, Schulden und Straffälligkeit nennt.

Sieben Verwendungen in fünf Ämtern. Die Verwendungen sind durchweg Legitimationsvorgänge —
der Nachweis, dass die handelnde Person die ist, die sie zu sein vorgibt.

*Durchsicht Los 2 (Amt 33) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los2-amt33.md`.*
