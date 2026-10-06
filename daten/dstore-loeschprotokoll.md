---
id: dstore-loeschprotokoll
bereich: intern
typ: datenspeicher
system: null
name: Löschprotokoll
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
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 5 Abs. 2, Art. 17
  - gesetz: NDSG
    artikel: § 3
  - gesetz: NArchG
    artikel: Anbietungspflicht vor Vernichtung
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach der Vernichtung
    hinweis: 'Frist wie in vvt-10-024 (Nachweis der ordnungsgemäßen Löschung).'
letzte-aktualisierung: '2026-10-05'
tags:
- Schriftgut
- Löschung
- Rechenschaftspflicht
---

# Löschprotokoll

## Definition

Nachweis über die Vernichtung von Akten und Datenträgern und die Löschung von Daten nach Ablauf der Aufbewahrungsfrist.

## Felder

- Aktenzeichen oder Bezeichnung des Bestands
- Art des Datenträgers
- Datum der Vernichtung oder Löschung
- Verfahren (Aktenvernichter, Dienstleister, Löschwerkzeug)
- ausführende Person oder Dienstleister
- Vernichtungs- oder Löschprotokoll, ggf. Zertifikat des Dienstleisters

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-10-024 und `proc-aktenvernichtung` nutzten bis dahin `dstore-verwaltungsakte`; die VVT vermerkte selbst, ein eigener Speicher für Löschprotokolle wäre präziser.

**Schutzstufe B.** Das Protokoll enthält Aktenzeichen und Namen der Ausführenden, nicht den Inhalt der vernichteten Akten.

**BSI-Vektoren.** Vertraulichkeit normal, Integrität hoch, Verfügbarkeit normal — die Integrität ist hoch, weil das Protokoll der Nachweis nach Art. 5 Abs. 2 DSGVO ist.

**Abgrenzung:**
- `dstore-verwaltungsakte`: Vorgangsakte in Bürgerverfahren, extern.
