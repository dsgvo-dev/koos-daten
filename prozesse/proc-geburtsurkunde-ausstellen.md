---
id: proc-geburtsurkunde-ausstellen
titel: Geburtsurkunde ausstellen
status: aktiv
bereich: extern
zustaendigeEinheit: oe-amt-31
zustaendigeRolle: ''
beteiligte:
- einheit: oe-amt-20
  aufgabe: ''
- rolle: antragstellende-person
  aufgabe: Initiator und Ergebnisempfänger
daten:
  input: []
  output: []
  datenspeicher:
  - id: dstore-geburtsurkunde
  - id: dstore-geburtsdaten-kind
  - id: dstore-personenstammdaten
  - id: dstore-registerbezug-personenstand
  - id: dstore-elternbezug-abstammung
  - id: dstore-geburtsurkunde-eltern
  - id: dstore-zweckgebundene-urkunde
  - id: dstore-antragsberechtigung-personenstand
regelungen:
- § 55 Absatz 1 Nummer 3 Personenstandsgesetz (PStG)
- § 59 Personenstandsgesetz (PStG)
- § 62 Personenstandsgesetz (PStG)
- § 50 Personenstandsverordnung (PStV)
leika_id: '99027002012000'
ozg_id: '10557'
letzte-aktualisierung: '2026-10-07'
---

# Geburtsurkunde ausstellen

## Prozessschritte

**01 Antrag stellen**  
*Antragstellende Person: Urkunde beantragen, Berechtigung nachweisen (§ 62 PStG)*

**02 Antragseingang prüfen**  
*Vollständigkeit der Unterlagen*

**03 Geburtenregister abgleichen**  
*Eintrag existiert?*

**04 Personalien verifizieren**  
*Berechtigung nach § 62 PStG*

**05 Urkunde erstellen**  
*Amtliche Form, Stempel, Unterschrift*

**06 Gebühren berechnen**  
*Je nach Anzahl der Exemplare*

**07 Aushändigung**  
*Persönlich oder per Post*

**08 Buchführung**  
*Vermerk in Akte, Statistik*

**09 Urkunde erhalten**  
*Antragstellende Person*


*Zusammengeführt am 06.10.2026 mit `proc-geburtsurkunde-beantragen` (ein Prozess je Leistung, FIM-Leistungsschlüssel 99027002012000; Entscheidung Martin 06.10.2026, Gruppe 6).*

*Am 07.10.2026 zusätzlich aufgegangen: `proc-geburtsurkunde-geburtenregister-ausstellen`, `proc-urkunde-geburtsurkunde-geburtenregister-beantragen` (gleiche Leistung ohne LeiKa-Schlüssel; Titel-Kandidat T1, Entscheidung Martin 07.10.2026).*
