---
id: proc-bussgeldbescheid-bearbeiten
titel: Bußgeldbescheid bearbeiten
status: aktiv
zustaendigeEinheit: oe-amt-32
zustaendigeRolle: Sachbearbeitung Ordnungswidrigkeiten
beteiligte:
  - einheit: oe-amt-34
    aufgabe: Zulieferung Fahrzeug- und Halterdaten bei Verkehrsverstößen

daten:
  input:
    - Anzeigen und Meldungen (Polizei, Außendienst, Einwohner)
    - Fahrzeug- und Halterdaten vom Straßenverkehrsamt
  output:
    - Bußgeldbescheid
    - Zahlungsaufforderung
  datenspeicher:
  - id: dstore-bussgeldakte
  - id: dstore-parkverstossanzeige

regelungen:
  - OWiG (Gesetz über Ordnungswidrigkeiten)
  - StVO (Straßenverkehrs-Ordnung)
  - BKatV (Bußgeldkatalog-Verordnung)
  - VwVfG (Verwaltungsverfahrensgesetz)

letzte-aktualisierung: 2026-04-23
---
# Bußgeldverfahren

## Prozessschritte

**01 Ordnungswidrigkeit dokumentieren**  
*Zeugen, Beweise*

**02 Rechtsgrundlage prüfen**  
*Welche Vorschrift verletzt?*

**03 Verwarnung aussprechen**  
*Schriftlich mit Begründung*

**04 Frist setzen**  
*Für Zahlung/Einspruch*

**05 Zahlungseingang prüfen**  
*Buchhaltung*

**06 Bei Nichtzahlung**  
*Vollstreckungsverfahren*

**07 Statistik führen**  
*Für Berichtswesen*


