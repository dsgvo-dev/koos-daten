---
id: proc-onboarding-neuer-mitarbeiter-innen
titel: Onboarding neuer Mitarbeiter/innen
status: aktiv
zustaendigeEinheit: oe-amt-11
zustaendigeRolle: Sachbearbeitung
beteiligte:
  - einheit: oe-amt-15
    aufgabe: IT-Arbeitsplatz einrichten, Zugriffsrechte vergeben, E-Mail-Konto anlegen
  - einheit: oe-hvb
    aufgabe: Persönliche Begrüßung, Dienstanweisungen und Schlüssel übergeben
  - einheit: oe-amt-1-4
    aufgabe: Datenschutz-Einweisung durchführen
daten:
  input:
    - Arbeitsvertrag, Einstellungsverfügung, Steuer-ID, Bankverbindung
  output:
    - Personalaktensatz, IT-Berechtigungsnachweis, Einweisungsnachweis
  datenspeicher:
    - id: dstore-personalakte
    - id: dstore-it-berechtigungsantrag
    - id: dstore-datenschutzeinweisung
    - id: dstore-arbeitsverhaeltnis-beschaeftigung
    - id: dstore-lebenslauf-qualifikationsnachweis
regelungen:
  - "Art. 88 DSGVO i.V.m. § 12 NDSG (Beschäftigtendatenschutz)"
  - "§§ 88, 94 NBG (Personalakte, Gesundheitsdaten)"
  - "§ 50 BeamtStG (Personalakte)"
  - "§ 1 TVöD/TV-L (Probezeit)"
  - "§ 86 NKomVG (Personalhoheit)"
  - "§§ 64–67 NPersVG (Mitbestimmung Personalrat)"
  - "DA Datenschutz § 4 (Einweisung)"
leika_id: null
ozg_id: null
letzte-aktualisierung: '2026-08-21'
---
# Onboarding neuer Mitarbeiter/innen

## Zweck

Der Prozess umfasst alle Schritte zwischen dem unterschriebenen Arbeitsvertrag und der vollständigen Integration der neuen Mitarbeiterin oder des neuen Mitarbeiters in die Verwaltung. Das Einstellungsverfahren (`proc-einstellungsverfahren`) ist abgeschlossen; das Onboarding stellt den Dienstantritt sicher, richtet die Arbeitsmittel ein, weist in Datenschutz und IT ein und begleitet die Probezeit. Betroffen sind alle neu eingestellten Beamtinnen und Beamten sowie Tarifbeschäftigte einschließlich Auszubildender. Rechtsgrundlage ist Art. 88 DSGVO i.V.m. § 12 NDSG in Verbindung mit §§ 88, 94 NBG, § 50 BeamtStG, dem TVöD/TV-L sowie §§ 64–67 NPersVG.

## Prozessschritte

**01 Dienstantritt vorbereiten**
*Nach Eingang des unterschriebenen Arbeitsvertrags und der Einstellungsverfügung veranlasst die Personalabteilung die Einrichtung des IT-Arbeitsplatzes (oe-amt-15), die Bestellung von Schlüssel und Dienstausweis sowie die Anforderung von Steuer-ID und Bankverbindung beim neuen Beschäftigten.*

**02 Persönliche Begrüßung und Übergabe**
*Am ersten Arbeitstag erfolgt die persönliche Begrüßung durch die Behördenleitung (oe-hvb). Die neuen Beschäftigten erhalten ihre Dienstanweisungen (DA Datenschutz, DA IT-Nutzung), den Dienstausweis und die Schlüssel. Die Übergabe wird dokumentiert.*

**03 Personalakte anlegen und ergänzen**
*Die Personalabteilung legt den Personalaktensatz nach §§ 88, 94 NBG an. Der Arbeitsvertrag, die Einstellungsverfügung, die Steuer-ID und die Bankverbindung werden zur Personalakte (dstore-personalakte) genommen. Die Bewerbungsunterlagen aus dem Einstellungsverfahren werden nach Ablauf der Aufbewahrungsfrist vernichtet.*

**04 Datenschutz-Einweisung und Verpflichtung**
*Die oder der Datenschutzbeauftragte (oe-amt-1-4) weist die neuen Beschäftigten in den Umgang mit personenbezogenen Daten ein. Die Einweisung umfasst die Pflichten nach Art. 5 DSGVO, die DA Datenschutz sowie die Folgen von Verstößen (Art. 82 DSGVO, § 203 StGB). Die Teilnahme wird in der dstore-datenschutzeinweisung dokumentiert.*

**05 IT-Einweisung und Zugriffsrechte**
*Die IT-Abteilung (oe-amt-15) richtet den Arbeitsplatz ein, vergibt die Zugriffsberechtigungen für die erforderlichen Fachverfahren, das E-Mail-Konto und das Dateiverzeichnis. Die neuen Beschäftigten werden in die Passwortrichtlinie und die DA IT-Nutzung eingewiesen. Der Berechtigungsnachweis wird in der dstore-it-berechtigungsantrag dokumentiert.*

**06 Einarbeitung und Probezeit**
*Die fachlich zuständige Führungskraft erstellt einen Einarbeitungsplan und benennt eine Patin oder einen Paten. Nach der Hälfte der Probezeit (§ 1 TVöD / § 2 NBG) findet ein Zwischengespräch statt. Bei mitbestimmungspflichtigen Maßnahmen wird der Personalrat nach §§ 64–67 NPersVG beteiligt.*

**07 Abschluss der Einarbeitung**
*Zum Ende der Probezeit erstellt die Führungskraft eine Probezeitbeurteilung. Bei Bewährung erfolgt die Übernahme in das Dauerbeschäftigungsverhältnis; bei Nichtbewährung werden die gesetzlichen Beendigungsfristen eingeleitet. Die Personalakte wird um die Beurteilung ergänzt.*

**Herkunft des Schrittblocks:** abgeleitet aus §§ 88, 94 NBG, § 50 BeamtStG, Art. 88 DSGVO i.V.m. § 12 NDSG, §§ 64–67 NPersVG sowie der DA Datenschutz, nicht aus einer Ablauferhebung im Amt 11.