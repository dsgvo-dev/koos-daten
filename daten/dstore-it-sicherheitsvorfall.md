---
id: dstore-it-sicherheitsvorfall
bereich: intern
typ: datenspeicher
system: null
name: IT-Sicherheitsvorfall
zuständige-einheit: oe-amt-15
personenbezug: ja
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 5 Abs. 2, Art. 32, Art. 33
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  - gesetz: NDIG
    artikel: IT-Sicherheit
  aufbewahrung:
    frist: 3 Jahre
    beginn: nach Abschluss der Bearbeitung
    hinweis: 'Frist wie in vvt-15-008 für Vorfallsdokumentation und forensische Berichte; System-Logs nach der Löschfrist des jeweiligen Systems.'
letzte-aktualisierung: '2026-10-05'
tags:
- IT-Sicherheit
- Incident Response
---

# IT-Sicherheitsvorfall

## Definition

Dokumentation von IT-Sicherheitsvorfällen von der Meldung über Analyse und Eindämmung bis zur Nachbereitung.

## Felder

- meldende Person (Name, System, Symptome, Zeitpunkt)
- betroffene Systeme und Konten
- Protokolldaten, IP-Adressen, Dateisysteminformationen
- forensische Daten (Arbeitsspeicher-Abbilder, Festplatten-Images)
- Schadsoftware-Muster
- Maßnahmen und Ergebnis
- Meldung an Datenschutzbeauftragte oder Aufsicht, soweit erforderlich

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-15-008 und `proc-itsicherheitsvorfall-melden` nutzten bis dahin `dstore-sicherheitsmangelmeldung`, extern.

**Schutzstufe D.** Forensische Kopien können beliebige personenbezogene Daten einschließlich besonderer Kategorien enthalten.

**BSI-Vektoren.** Vertraulichkeit hoch, Integrität hoch, Verfügbarkeit normal — Vertraulichkeit hoch wegen der forensischen Inhalte; Integrität hoch, weil die Dokumentation Beweis- und Nachweisfunktion hat.

**Abgrenzung:**
- `dstore-stoerungsmeldung-intern`: gewöhnliche Störungen ohne Sicherheitsbezug.
