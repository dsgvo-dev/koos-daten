---
id: proc-gebaeudeverwaltung
titel: Kommunale Gebäude verwalten (Objektverwaltung)
status: aktiv
bereich: intern
zustaendigeEinheit: oe-amt-65
zustaendigeRolle: sachbearbeiter
beteiligte:
- einheit: oe-amt-10
  aufgabe: Störungsmeldungen, Schlüsselverwaltung, Beschaffung
- einheit: oe-amt-20
  aufgabe: Zahlungen und Anlagenbuchhaltung
daten:
  input: []
  output: []
  datenspeicher:
  - id: dstore-beschaffungsvorgang
  - id: dstore-stoerungsmeldung-intern
regelungen:
- '§ 124 Abs. 2 NKomVG (Vermögensgegenstände pfleglich und wirtschaftlich verwalten und ordnungsgemäß nachweisen)'
leika_id: ''
ozg_id: ''
letzte-aktualisierung: '2026-10-06'
---
# Kommunale Gebäude verwalten (Objektverwaltung)

Rahmenprozess für die eigenen Gebäude der Kommune (Rathaus, Verwaltungsgebäude, Schulen, Bürgerhäuser). Teilaufgaben mit eigenem Prozess: `proc-gebaeudereinigung`, `proc-heizung-warten`, `proc-gebaeudesanierung-planen`, `proc-schluesselverwaltung`, `proc-stoerung-haustechnik`. Die Überlassung von Räumen an Externe ist ein eigener, externer Prozess (`proc-raeume-oeffentlicher-einrichtungen-ueberlassen`); die städtischen Mietwohnungen laufen über `proc-mietvertrag-fuer-staedtische-wohnung`.

## Prozessschritte

**01 Gebäudebestand führen**  
*Objekte, Flächen, nutzende Organisationseinheiten und Objektverantwortliche erfassen und aktuell halten.*

**02 Bewirtschaftung steuern**  
*Verträge mit Dienstleistern für Reinigung, Wartung und Energie abschließen und überwachen (siehe `proc-gebaeudereinigung`, `proc-heizung-warten`).*

**03 Instandhaltung planen**  
*Mängel aus Störungsmeldungen und Begehungen bewerten und beheben; größere Maßnahmen an `proc-gebaeudesanierung-planen` übergeben.*

**04 Belegung steuern**  
*Raumbedarf der Ämter feststellen, Räume zuweisen, Umzüge planen.*

**05 Zugang regeln**  
*Schließberechtigungen über `proc-schluesselverwaltung`.*

**06 Kosten erfassen und Bestand nachweisen**  
*Bewirtschaftungs- und Instandhaltungskosten erfassen; Gebäude als Vermögensgegenstände nach § 124 Abs. 2 NKomVG nachweisen.*

*Quelle: neu gefasst 2026-10-06 (Entwurf Claude, Freigabe Martin); vorher eine leere Vorlage mit den sechs Standardschritten.*
