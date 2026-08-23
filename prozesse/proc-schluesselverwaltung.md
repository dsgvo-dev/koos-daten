---
id: proc-schluesselverwaltung
titel: Schlüssel verwalten (Ausgabe, Rücknahme, Verlust)
status: aktiv
zustaendigeEinheit: oe-amt-10
zustaendigeRolle: Sachbearbeitung
beteiligte:
  - einheit: oe-amt-11
    aufgabe: Mitteilung über Einstellung/Ausscheiden von Beschäftigten an das Hauptamt
  - einheit: oe-amt-15
    aufgabe: Verwaltung elektronischer Schließanlagen (Transponder, Chipkarten)
  - einheit: oe-hvb
    aufgabe: Genehmigung von Sonderberechtigungen (Hauptschlüssel, Außendienst)
daten:
  input:
    - Schlüsselantrag mit Begründung, Freigabe der Fachverantwortlichen
  output:
    - Empfangsbestätigung, Eintrag im Schlüsselverzeichnis
  datenspeicher:
    - id: dstore-schluesselverwaltung
    - id: dstore-vollmacht-vertretung-berechtigung
regelungen:
  - "Dienstanweisung Schlüsselverwaltung (Hausrecht)"
  - "§ 86 NKomVG (Verwaltungsorganisation)"
  - "Sicherheitsrichtlinie Gebäude (Zutrittskontrolle)"
  - "Art. 6 Abs. 1 lit. e DSGVO, § 3 NDSG (Aufgabenerfüllung)"
leika_id: null
ozg_id: null
letzte-aktualisierung: '2026-08-22'
---
# Schlüssel verwalten (Ausgabe, Rücknahme, Verlust)

## Zweck

Die Verwaltung von Schlüsseln und Schließanlagen umfasst die Ausgabe, Rücknahme und Verlustbearbeitung von mechanischen und elektronischen Schlüsseln (Transponder, Chipkarten) für die Diensträume der Verwaltung. Der Prozess dient der Zutrittskontrolle und der Sicherheit der Gebäude und der darin verarbeiteten Daten. Betroffen sind alle Beschäftigten sowie externe Dienstleister mit Zugangsberechtigung. Die Daten werden nach Art. 6 Abs. 1 lit. e DSGVO i.V.m. § 3 NDSG zur Aufgabenerfüllung verarbeitet.

## Prozessschritte

**01 Schlüssel beantragen und genehmigen**
*Der oder die Beschäftigte beantragt einen Schlüssel beim Hauptamt (oe-amt-10) mit Begründung (Zimmer, Gebäude, Außendienst). Die fachlich zuständige Führungskraft genehmigt die Ausgabe. Bei Sonderberechtigungen (Hauptschlüssel, Generalschlüssel) ist die Freigabe der Behördenleitung (oe-hvb) erforderlich. Die Personalabteilung (oe-amt-11) meldet Einstellungen und Versetzungen proaktiv an das Hauptamt.*

**02 Schlüssel ausgeben und quittieren**
*Das Hauptamt gibt den Schlüssel oder Transponder gegen Unterschrift aus. Der Eintrag im Schlüsselverzeichnis umfasst: Schlüsselnummer/Transponder-ID, Name der empfangenden Person, Datum der Ausgabe, ausgebende Person und Raumzuordnung. Bei Chipkarten erfolgt die Aktivierung durch die IT-Abteilung (oe-amt-15).*

**03 Schlüssel zurücknehmen**
*Bei Ausscheiden, Versetzung oder Wegfall des Bedarfs wird der Schlüssel unverzüglich an das Hauptamt zurückgegeben. Die Rücknahme wird im Schlüsselverzeichnis dokumentiert. Bei elektronischen Schlüsseln wird die Berechtigung durch die IT-Abteilung deaktiviert. Die Personalabteilung informiert das Hauptamt über bevorstehende Austritte.*

**04 Schlüsselverlust bearbeiten**
*Bei Verlust eines Schlüssels erfolgt die unverzügliche Meldung durch die oder den Beschäftigten an das Hauptamt. Das Hauptamt sperrt den Schlüssel und veranlasst bei mechanischen Schließanlagen die Umstellung der betroffenen Zylinder. Der Verlust wird im Schlüsselverlustregister dokumentiert. Bei Diebstahl ist zusätzlich eine Strafanzeige zu erstatten.*

**05 Bestand prüfen und nachhalten**
*Das Hauptamt führt fortlaufend das Schlüsselverzeichnis. Mindestens einmal jährlich wird ein Soll-Ist-Abgleich der ausgegebenen Schlüssel durchgeführt. Abweichungen werden nachverfolgt und dokumentiert.*

**Herkunft des Schrittblocks:** abgeleitet aus der Dienstanweisung Schlüsselverwaltung, der Sicherheitsrichtlinie Gebäude, § 86 NKomVG sowie Art. 6 Abs. 1 lit. e DSGVO i.V.m. § 3 NDSG, nicht aus einer Ablauferhebung im Amt 10.