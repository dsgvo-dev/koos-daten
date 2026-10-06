---
id: dstore-stoerungsmeldung-intern
bereich: intern
typ: datenspeicher
system: null
name: Störungsmeldung intern
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
    artikel: Art. 6 Abs. 1 lit. e
  - gesetz: NDSG
    artikel: § 12 Abs. 1
  aufbewahrung:
    frist: 3 Jahre
    beginn: nach Abschluss der Störungsbearbeitung
    hinweis: 'Frist wie in vvt-10-028 und vvt-15-005.'
letzte-aktualisierung: '2026-10-05'
tags:
- Haustechnik
- IT
- Störung
---

# Störungsmeldung intern

## Definition

Meldungen von Beschäftigten über Störungen der Haustechnik (Heizung, Licht, Sanitär, Aufzug) und der IT (Hardware, Software, Zugang, Netzwerk) und deren Bearbeitung.

## Felder

- meldende Person und dienstliche Kontaktdaten
- Art, Ort und Umfang der Störung
- betroffene Systeme oder Anlagen
- Bearbeitung und Lösung
- Zeitpunkte von Meldung und Erledigung

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-10-028, vvt-15-005, `proc-stoerung-haustechnik` und `proc-stoerung-it` nutzten bis dahin `dstore-sicherheitsmangelmeldung` (Mängel im öffentlichen Raum) und `dstore-beschwerde-anregungsdaten` (Bürgerbeschwerden), beide extern.

**Schutzstufe B.** Dienstliche Angaben der meldenden Person.

**BSI-Vektoren.** Vertraulichkeit normal, Integrität normal, Verfügbarkeit normal — keine besonderen Anforderungen.

**Abgrenzung:**
- `dstore-it-sicherheitsvorfall`: Sicherheitsvorfälle mit forensischen Daten.
- `dstore-sicherheitsmangelmeldung`: Mängel im öffentlichen Raum, extern.
