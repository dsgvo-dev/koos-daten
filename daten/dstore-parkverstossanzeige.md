---
id: dstore-parkverstossanzeige
typ: datenspeicher
system: null
name: Parkverstoßanzeige
datenkategorie: Verkehr & Vollzug
zuständige-einheit: oe-amt-34
bpmn:
  typ: datenobjekt
klassifizierung:
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeit: vertraulich
  rechtsgrundlagen:
  - gesetz: StVO
  - gesetz: OWiG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: 2026-04-09
tags:
- Parkverstoß
- Anzeige
- Kennzeichen
---

# Parkverstoßanzeige

## Definition

Daten zu gemeldeten Parkverstößen im öffentlichen Verkehrsraum.

## Felder

- Kennzeichen
- Ort
- Zeitpunkt
- Verstoßart
- Fotobeleg
- Meldende Person

## Hinweise

Aus weiteren niedersächsischen Serviceportalen (Oldenburg, Osnabrück, Landkreis Hameln-Pyrmont, Hannover) abgeleiteter Datentyp. Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.
