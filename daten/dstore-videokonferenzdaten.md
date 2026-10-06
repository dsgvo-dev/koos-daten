---
id: dstore-videokonferenzdaten
bereich: intern
typ: datenspeicher
system: null
name: Videokonferenzdaten
zuständige-einheit: oe-amt-15
personenbezug: ja
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. e, Art. 6 Abs. 1 lit. a (Aufzeichnung)
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  aufbewahrung:
    frist: Aufzeichnung höchstens 30 Tage
    beginn: nach der Besprechung
    hinweis: 'Frist wie in vvt-15-001; Einwilligungen und Widerrufe 12 Monate nach Löschung der Aufzeichnung.'
letzte-aktualisierung: '2026-10-05'
tags:
- Videokonferenz
- Kommunikation
---

# Videokonferenzdaten

## Definition

Daten, die bei Videokonferenzen der Verwaltung mit Beschäftigten und externen Teilnehmenden entstehen.

## Felder

- Teilnehmende (Name, Organisationseinheit)
- Bild und Ton während der Konferenz
- Chat- und Textnachrichten
- Inhalte der Bildschirmfreigabe
- technische Verbindungsdaten
- ausnahmsweise Aufzeichnung mit Einwilligungen und Widerrufen

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-15-001 und `proc-videokonferenz-fuer-interne-besprechungen-bereitstellen` nutzten bis dahin `dstore-bild-und-tonaufnahmen` (Öffentlichkeitsarbeit) und `dstore-kontaktdaten`, beide extern.

**Schutzstufe C.** Bild, Ton und Chat können Inhalte jeder Art enthalten; Aufzeichnungen nur ausnahmsweise.

**BSI-Vektoren.** Vertraulichkeit normal, Integrität normal, Verfügbarkeit normal — keine besonderen Anforderungen.

**Abgrenzung:**
- `dstore-bild-und-tonaufnahmen`: Aufnahmen für Öffentlichkeitsarbeit und Bildarchiv, extern.
