---
id: dstore-unternehmens-und-registerdaten
typ: datenspeicher
system: null
name: Unternehmens- und Registerdaten
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: HGB
  - gesetz: BGB
  - gesetz: GewO
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-12'
tags:
- Handelsregister
- Vereinsregister
- juristische Person
- Vertreter
- Satzung
---



# Unternehmens- und Registerdaten

## Definition

Daten zu juristischen Personen, Vereinen und deren registerrechtlicher Einordnung.

## Felder

- Rechtsform
- Handelsregisterauszug
- Vereinsregisterauszug
- gesetzlicher Vertreter
- Satzung
- Unternehmensname

## Klassifizierung

- Schutzstufe: B
- Schutzbedarf: normal
- Vertraulichkeit: intern
- BPMN-Typ: datenspeicher

## Rechtsgrundlagen

- HGB
- BGB
- GewO

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Spielhallen, Erlaubnis
- Veranstaltung eines Jahr- oder Spezialmarktes: Festsetzung

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Organisationsdaten werden separat von Zuverlässigkeitsauskünften geführt, um Unternehmen und Personen trennscharf abzubilden.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** Der Speicher wird in so vielen Verfahren geführt, dass ein Ausfall nicht ein Verfahren verzögert, sondern den Publikumsverkehr insgesamt zum Erliegen bringt. Das ist der Maßstab des BSI: erhebliche Beeinträchtigung der Aufgabenerfüllung.

25 Verwendungen quer durch Gewerbe-, Vergabe- und Ordnungsrecht.

## Schutzstufe geprüft 2026-08-12

**Herabgestuft von C auf B.** Der gesamte Inhalt ist von Gesetzes wegen öffentlich einsehbar:

- **§ 9 Abs. 1 HGB** — die Einsicht in das Handelsregister und die zu ihm eingereichten Dokumente ist jedem zu Informationszwecken gestattet.
- **§ 79 Abs. 1 BGB** — die Einsicht in das Vereinsregister und die von dem Verein zum Register eingereichten Schriftstücke ist jedem gestattet.

Personenbezug hat allein der gesetzliche Vertreter, und zwar in seiner Funktion, nicht als Privatperson. Eine unbefugte Offenbarung nimmt niemandem etwas, was nicht ohnehin abrufbar wäre.

**Warum B und nicht A.** Stufe A setzt voraus, dass die betroffene Person die Daten *selbst frei zugänglich gemacht* hat — Telefonverzeichnis, eigene Webseite. Eine Registereintragung ist Pflicht, keine freiwillige Veröffentlichung, und der kommunale Auszug liegt nicht offen. B trifft es: nicht frei zugänglich, Missbrauch ohne besondere Beeinträchtigung.

**Wirksamster Einzelposten des Loses.** 25 Verwendungen in acht Ämtern. Eine Stufe C hätte für Daten, die kostenfrei abrufbar sind, Maßnahmen verlangt und damit die Steuerungswirkung der Einstufung entwertet.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
