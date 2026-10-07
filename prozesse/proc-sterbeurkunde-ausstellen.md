---
id: proc-sterbeurkunde-ausstellen
titel: Sterbeurkunde ausstellen
status: aktiv
bereich: extern
zustaendigeEinheit: oe-amt-31
zustaendigeRolle: ''
beteiligte:
- einheit: oe-amt-33
  aufgabe: ''
- einheit: oe-amt-15
  aufgabe: ''
- einheit: oe-amt-20
  aufgabe: ''
- rolle: antragstellende-person
  aufgabe: Initiator und Ergebnisempfänger
daten:
  input: []
  output: []
  datenspeicher:
  - id: dstore-personenstammdaten
  - id: dstore-registerbezug-personenstand
  - id: dstore-sterbeurkunde
regelungen:
- § 55 Absatz 1 Nummer 4 Personenstandsgesetz (PStG)
- § 60 Personenstandsgesetz (PStG)
- § 62 Personenstandsgesetz (PStG)
- § 55 Personenstandsgesetz (PStG)
leika_id: '99101004012000'
ozg_id: '10237'
letzte-aktualisierung: '2026-10-07'
---

# Sterbeurkunde ausstellen

## Prozessschritte

**01 Antrag stellen**  
*Antragstellende Person: Urkunde beantragen, Berechtigung nachweisen (§ 62 PStG)*

**02 Antragseingang prüfen**  
*Vollständigkeit der Unterlagen*

**03 Sterberegister abgleichen**  
*Eintrag existiert?*

**04 Berechtigung prüfen**  
*Rechtsgrundlage: § 62 PStG*

**05 Urkunde erstellen**  
*Amtliche Form, Stempel, Unterschrift (§ 60 PStG)*

**06 Gebühren berechnen**  
*Je nach Anzahl der Exemplare*

**07 Aushändigung**  
*Persönlich oder per Post*

**08 Urkunde erhalten**  
*Antragstellende Person*


## Korrektur 2026-08-03

Englischsprachige Dubletten aus der Regelungsliste entfernt. Es handelt sich um Übersetzungen bereits vorhandener deutscher Fundstellen aus dem Quellkatalog, nicht um eigene Normen:
- § 55 Civil Status Act (PStG)
- § 60 Civil Status Act (PStG)

*Zusammengeführt am 06.10.2026 mit `proc-sterbeurkunde-beantragen` (ein Prozess je Leistung, FIM-Leistungsschlüssel 99101004012000; Entscheidung Martin 06.10.2026, Gruppe 26).*

*Am 07.10.2026 zusätzlich aufgegangen: `proc-urkunde-sterbeurkunde-beantragen` (gleiche Leistung ohne LeiKa-Schlüssel; Titel-Kandidat T3, Entscheidung Martin 07.10.2026).*
