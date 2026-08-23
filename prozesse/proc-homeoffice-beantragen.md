---
id: proc-homeoffice-beantragen
titel: Homeoffice / Mobiles Arbeiten beantragen
status: aktiv
zustaendigeEinheit: oe-amt-11
zustaendigeRolle: Sachbearbeitung
beteiligte:
  - einheit: oe-amt-15
    aufgabe: Bereitstellung von VPN-Zugang, Remote-Zugriff, Dienstgeräten für Homeoffice
  - einheit: oe-amt-1-4
    aufgabe: Datenschutzrechtliche Beratung, Freigabe der TOM für mobiles Arbeiten
beteiligte_personalrat:
  - einheit: oe-personalrat
    aufgabe: Mitbestimmung nach §§ 64–67 NPersVG (Einführung/Änderung der Homeoffice-Regelungen)
daten:
  input:
    - Antrag der/des Beschäftigten (Name, Tätigkeitsbereiche, gewünschte Tage/Umfang, Adresse des Arbeitsortes)
  output:
    - Genehmigungsbescheid, IT-Berechtigungsantrag (VPN), Eintrag in Personalakte
  datenspeicher:
    - id: dstore-personalakte
    - id: dstore-arbeitsverhaeltnis-beschaeftigung
    - id: dstore-it-berechtigungsantrag
regelungen:
  - "Art. 88 DSGVO i.V.m. § 12 NDSG (Beschäftigtendatenschutz)"
  - "Art. 6 Abs. 1 lit. e DSGVO, § 3 NDSG (Aufgabenerfüllung)"
  - "§ 86 NKomVG (Personalhoheit)"
  - "§ 5 ArbSchG (Gefährdungsbeurteilung des häuslichen Arbeitsplatzes)"
  - "Dienstvereinbarung Homeoffice / Mobiles Arbeiten (§ 78 NPersVG)"
  - "§§ 64–67 NPersVG (Mitbestimmung)"
  - "§ 16 TVöD/TV-L (Arbeitszeit, soweit anwendbar)"
  - "LfD Niedersachsen, Hilfestellung Datenschutz im Homeoffice (12/2023)"
leika_id: null
ozg_id: null
letzte-aktualisierung: '2026-08-23'
---
# Homeoffice / Mobiles Arbeiten beantragen

## Zweck

Antragstellung, Prüfung und Genehmigung von Homeoffice oder mobilem Arbeiten für Beschäftigte der Verwaltung. Der Prozess umfasst die Prüfung der Tätigkeitseignung, die Gefährdungsbeurteilung des häuslichen Arbeitsplatzes, die Bereitstellung der IT-Infrastruktur (VPN, Remote-Zugriff, Dienstgeräte) sowie die datenschutzrechtliche Freigabe.

**Anlaufstelle für Anträge:** Personalabteilung (oe-amt-11). IT-Bereitstellung und Gefährdungsbeurteilung werden parallel durch IT (oe-amt-15) und Fachvorgesetzte bearbeitet.

## Prozessschritte

**01 Antrag einreichen**
*Die oder der Beschäftigte reicht den Homeoffice-Antrag bei der Personalabteilung (oe-amt-11) ein. Der Antrag enthält: Name, Tätigkeitsbereiche, die für Homeoffice geeignet sind, gewünschter Umfang (Tage pro Woche/Monat), Adresse des häuslichen Arbeitsplatzes, gewünschte IT-Ausstattung.*

**02 Tätigkeitseignung prüfen**
*Die Personalabteilung prüft gemeinsam mit der oder dem Fachvorgesetzten, ob die Tätigkeit für Homeoffice geeignet ist (keine zwingende Präsenz erforderlich, Zugriff auf Fachverfahren über VPN möglich, Vertraulichkeit der Daten gewährleistet). Nicht geeignet sind Tätigkeiten mit Publikumsverkehr, Zugang zu VS-Verschlusssachen oder solche, die zwingend Dienstgeräte vor Ort erfordern.*

**03 Gefährdungsbeurteilung des häuslichen Arbeitsplatzes**
*Die oder der Fachvorgesetzte führt gemeinsam mit der oder dem Beschäftigten die Gefährdungsbeurteilung des häuslichen Arbeitsplatzes nach § 5 ArbSchG durch: Beurteilung des Bildschirmarbeitsplatzes, der ergonomischen Bedingungen, Beleuchtung, Lärm, Brandschutz. Die Beurteilung wird dokumentiert und zur Personalakte genommen.*

**04 IT-Infrastruktur bereitstellen**
*Die IT-Abteilung (oe-amt-15) richtet den VPN-Zugang und ggf. den Remote-Zugriff auf die erforderlichen Fachverfahren ein. Die oder der Beschäftigte erhält die erforderlichen Dienstgeräte (Laptop, Monitor, Headset, ggf. Diensthandy) und wird in die sichere Nutzung eingewiesen (VPN-Nutzung, verschlüsselte Datenspeicherung, Bildschirmsperre, Mitnahmeverbot von Akten in Papierform). Die Einweisung wird in der dstore-it-berechtigungsantrag dokumentiert.*

**05 Genehmigung erteilen**
*Die Personalabteilung erteilt die Genehmigung schriftlich. Die Genehmigung enthält: Umfang (Tage/Woche), Laufzeit (befristet oder unbefristet), Auflagen (Erreichbarkeit, Arbeitszeitdokumentation), Widerrufsvorbehalt. Die Genehmigung wird zur Personalakte genommen.*

**06 Datenschutz-Einweisung bestätigen**
*Die oder der Beschäftigte bestätigt die Kenntnisnahme der Datenschutzregelungen für Homeoffice (Umgang mit personenbezogenen Daten, Verbot der Mitnahme von Papierakten, Verschlüsselung, Meldepflicht bei IT-Sicherheitsvorfällen) nach der LfD Niedersachsen-Hilfestellung. Die Bestätigung wird dokumentiert.*

**07 Widerruf oder Änderung**
*Bei Wegfall der Voraussetzungen, Änderung der Tätigkeit oder auf Antrag der/des Beschäftigten wird die Homeoffice-Genehmigung angepasst oder widerrufen. Der Widerruf ist schriftlich zu erklären. Die IT-Abteilung entzieht die Remote-Zugriffe. Die Änderung wird zur Personalakte genommen.*

**Herkunft des Schrittblocks:** abgeleitet aus Art. 88 DSGVO i.V.m. § 12 NDSG, § 5 ArbSchG, der LfD Niedersachsen-Hilfestellung Datenschutz im Homeoffice, der Dienstvereinbarung Homeoffice sowie der DA IT-Nutzung, nicht aus einer Ablauferhebung im Amt 11.