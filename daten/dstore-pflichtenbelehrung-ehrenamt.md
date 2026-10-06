---
id: dstore-pflichtenbelehrung-ehrenamt
bereich: extern
typ: datenspeicher
system: null
name: Pflichtenbelehrung Ehrenamt
zuständige-einheit: oe-amt-10
personenbezug: ja
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c
  - gesetz: NDSG
    artikel: § 3
  - gesetz: NKomVG
    artikel: § 40, § 43
  aufbewahrung:
    frist: Dauer der Tätigkeit, danach 10 Jahre
    beginn: Ende der ehrenamtlichen Tätigkeit
    hinweis: 'Frist wie in vvt-10-011.'
letzte-aktualisierung: '2026-10-05'
tags:
- Ehrenamt
- Verschwiegenheit
---

# Pflichtenbelehrung Ehrenamt

## Definition

Nachweis, dass ehrenamtlich Tätige nach § 43 NKomVG auf die gewissenhafte Erfüllung ihrer Pflichten und die Amtsverschwiegenheit (§ 40 NKomVG) hingewiesen wurden.

## Felder

- Name der ehrenamtlich tätigen Person
- ehrenamtliche Funktion
- Datum der Belehrung
- belehrende Person
- Unterschrift oder Bestätigung

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-10-011 nutzte bis dahin `dstore-datenschutzeinweisung`, die Verpflichtung der Beschäftigten (intern).

**Schutzstufe B.** Nur Belehrungsnachweis.

**BSI-Vektoren.** Vertraulichkeit normal, Integrität normal, Verfügbarkeit normal — keine besonderen Anforderungen.

**Abgrenzung:**
- `dstore-datenschutzeinweisung`: Verpflichtung der Beschäftigten, intern.
- `dstore-ehrenamtsdaten`: übrige Angaben zur ehrenamtlichen Tätigkeit.
