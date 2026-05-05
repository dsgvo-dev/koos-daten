---
id: dstore-debitoren-kreditorendaten
typ: datenspeicher
system: null
name: Debitoren- und Kreditorendaten
datenkategorie: Finanzen & Zahlung
zuständige-einheit: oe-amt-20
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: HGB
  - gesetz: KomHKVO
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Debitor
- Kreditor
- Buchhaltung
---

# Debitoren- und Kreditorendaten

## Definition

Stamm- und Buchungsdaten von Zahlungspflichtigen und Zahlungsempfängern.

## Felder

- Name oder Firma
- Buchungskonto
- Anschrift
- Steuernummer
- Zahlungsbedingung
- Status

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
