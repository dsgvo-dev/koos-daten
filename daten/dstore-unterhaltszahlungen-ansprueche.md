---
id: dstore-unterhaltszahlungen-ansprueche
typ: datenspeicher
system: null
name: Unterhaltszahlungen und Unterhaltsansprüche
datenkategorie: Familie & Soziales
zuständige-einheit: oe-amt-50
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: BGB
  - gesetz: UVG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Unterhalt
- Anspruch
- Zahlung
---



# Unterhaltszahlungen und Unterhaltsansprüche

## Definition

Daten zu geschuldetem, gezahltem oder erhaltenem Unterhalt.

## Felder

- Unterhaltspflichtige Person
- Berechtigte Person
- Zahlbetrag
- Zeitraum
- Titel oder Vereinbarung
- Zahlungsnachweis

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Der Bestand ist Grundlage einer Entscheidung über einen Menschen. Eine unbemerkte Verfälschung führt zu einer falschen Entscheidung, die für die betroffene Person unmittelbare Folgen hat und im Nachhinein kaum aufzuklären ist.

Der Bestand trägt Zahlungsansprüche und Rückforderungen. Ein falscher Stand belastet oder entlastet die falsche Person.

## Schutzstufe geprüft 2026-08-10

**C → D.** Die Datenart trägt zwei Seiten. Bei der berechtigten Person offenbart sie Trennung und regelmäßig das Alleinerziehen; beim Unterhaltsvorschuss nach dem UVG zusätzlich, dass die Zahlungen ausbleiben. **Bei der pflichtigen Person offenbart sie das Gegenstück:** Titel, Rückstand und den Übergang des Anspruchs auf das Land nach § 7 UVG -- also eine öffentliche Forderung, die vollstreckt wird. Schulden und Vollstreckung sind im LfD-Konzept Stufe D.
