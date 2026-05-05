---
id: dstore-servicekonto-nutzeridentitaet
typ: datenspeicher
system: null
name: Servicekonto und Nutzeridentität
datenkategorie: Digitale Verwaltung
zuständige-einheit: oe-amt-1-6
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: OZG
  - gesetz: EGovG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Servicekonto
- Login
- Nutzer
---

# Servicekonto und Nutzeridentität

## Definition

Konten- und Identitätsdaten eines verwaltungsbezogenen Online-Servicekontos.

## Felder

- Kontotyp
- Nutzerkennung
- Authentifizierungsniveau
- Verknüpfte Person
- Kontaktadresse
- Registrierungsdatum

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
