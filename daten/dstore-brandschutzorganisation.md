---
id: dstore-brandschutzorganisation
bereich: intern
typ: datenspeicher
system: null
name: Brandschutzorganisation
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
    artikel: § 12 Abs. 1
  - gesetz: ArbSchG
    artikel: § 10
  - gesetz: ArbStättV
    artikel: § 4 Abs. 4
  - gesetz: DGUV Vorschrift 1
    artikel: § 22
  aufbewahrung:
    frist: 5 Jahre
    beginn: Unterweisungsnachweise nach Ausscheiden; Evakuierungsprotokolle nach Erstellung
    hinweis: 'Frist wie in vvt-10-026; Brandschutzordnung in der jeweils aktuellen Fassung.'
letzte-aktualisierung: '2026-10-05'
tags:
- Brandschutz
- Arbeitsschutz
- Evakuierung
---

# Brandschutzorganisation

## Definition

Organisation des betrieblichen Brandschutzes und der Evakuierung in den Dienstgebäuden.

## Felder

- Brandschutzbeauftragte und Evakuierungshelfende (Name, Kontaktdaten)
- Unterweisungsnachweise der Beschäftigten
- Evakuierungs- und Räumungsübungsprotokolle
- Brandschutzordnung

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-10-026 und `proc-brandschutz-intern` nutzten bis dahin `dstore-brandschutznachweis` und `dstore-feuerwehrzufahrt-aufstellflaechen` aus dem Bauordnungsrecht; die VVT nannte sie selbst Behelfspeicher.

**Schutzstufe B.** Dienstliche Angaben.

**BSI-Vektoren.** Vertraulichkeit normal, Integrität normal, Verfügbarkeit normal — keine besonderen Anforderungen.

**Abgrenzung:**
- `dstore-brandschutznachweis`: Nachweis im Baugenehmigungsverfahren, extern.
