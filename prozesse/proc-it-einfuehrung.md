---
id: proc-it-einfuehrung
titel: IT-Verfahren einführen (Beschaffung, Prüfung, Freigabe, Produktivbetrieb)
status: aktiv
zustaendigeEinheit: oe-amt-10
zustaendigeRolle: fachverantwortliche
beteiligte:
- rolle: datenschutzbeauftragte
  phase: 2,3,6
  aufgabe: DSFA-Prüfung, AVV-Prüfung, VVT-Eintrag, Beratung
- rolle: informationssicherheitsbeauftragte
  phase: 2,3,6
  aufgabe: TOM-Prüfung, Schutzbedarf, Risikoanalyse
- rolle: personalrat
  phase: 3,6
  aufgabe: Mitbestimmung bei Einführung und bei wesentlichen Änderungen
- rolle: it-abteilung
  phase: 1,2,3,4,5,6
  aufgabe: Technische Prüfung, Implementierung, Berechtigungskonzept
- rolle: rechtsabteilung
  phase: '3'
  aufgabe: Vertragsprüfung (AVV, EVB-IT, Dienstleistungsvertrag)
- rolle: beschaffungsstelle
  phase: '3'
  aufgabe: Vergabeverfahren nach Vergabeordnung
daten:
  datenspeicher:
  - dstore-it-berechtigungsantrag
  - dstore-datenschutzeinweisung
  - dstore-vergabe-auftragsbezug
regelungen:
- Art. 5 DSGVO (Grundsätze)
- Art. 25 DSGVO (Privacy by Design/Default)
- Art. 28 DSGVO (Auftragsverarbeitung)
- Art. 32 DSGVO (Sicherheit der Verarbeitung)
- Art. 35 DSGVO (Datenschutz-Folgenabschätzung)
- Art. 30 DSGVO (Verzeichnis von Verarbeitungstätigkeiten)
- § 67 Abs. 1 Nr. 2 NPersVG (§ 75 Abs. 3 Nr. 17 BPersVG)
- BSI-Standard 200-2 (IT-Grundschutz-Methodik)
- Vergabeordnung (UVgO/VgV)
leika_id: ''
ozg_id: ''
letzte-aktualisierung: '2026-08-04'
---

# IT-Verfahren einführen

## Prozessschritte

**01 Bedarf anmelden**  
*Fachverantwortliche/r meldet Bedarf für neues IT-Verfahren schriftlich bei IT-Abteilung und DSB. Der Antrag enthält: Bezeichnung, Zweck, Datenkategorien, betroffene Personenkreise, Anzahl Nutzer, geplanter Termin, Angabe zu externem Betrieb.*

**02 Vorprüfung durch IT-Abteilung**  
*IT-Abteilung prüft technische Integration, Schnittstellen zu anderen Systemen, Kompatibilität mit Sicherheitsstandards, benötigte Hard- und Software-Ressourcen. Ergebnis: Technische Machbarkeit wird dokumentiert.*

**03 Datenschutzprüfung durch DSB**  
*DSB prüft: Erforderlichkeit einer DSFA nach Art. 35 DSGVO. Bei hohem Risiko (Art. 9-Daten, umfangreiche Überwachung, KI mit Personenbezug, biometrische Daten) wird die DSFA vor der Freigabe durchgeführt. DSB bewertet Privacy by Design/Default nach Art. 25 DSGVO. Ergebnis: Datenschutzrechtliche Bewertung liegt vor.*

**04 Sicherheitsprüfung durch ISB**  
*ISB prüft: Angemessenheit der TOM nach Art. 32 DSGVO, Schutzbedarf des Verfahrens (normal/hoch), Notwendigkeit einer Risikoanalyse. Ergebnis: Sicherheitstechnische Bewertung liegt vor.*

**05 Vertrags- und AVV-Prüfung**  
*Rechtsabteilung und DSB prüfen: Liegt Auftragsverarbeitung nach Art. 28 DSGVO vor? → AVV erstellen/prüfen. Liegt gemeinsame Verantwortlichkeit nach Art. 26 vor? → Vereinbarung schließen. Ist der Dienstleister eigenständig verantwortlich? → Vertragliche Absicherung. EVB-IT-Vertragsmuster verwenden. Ergebnis: Verträge sind geprüft und geschlossen.*

**06 Freigabe durch IT, DSB, ISB**  
*Freigabe wird dokumentiert. Voraussetzungen: Datenschutzrechtliche Unbedenklichkeit, sicherheitstechnische Bewertung, AVV geschlossen, VVT-Eintrag vorbereitet, Berechtigungskonzept im Entwurf. Personalrat wird informiert und bei Mitbestimmungstatbestand beteiligt (§ 67 Abs. 1 Nr. 2 NPersVG).*

**07 Beschaffung durchführen**  
*Beschaffungsstelle leitet Vergabeverfahren nach Vergabeordnung ein. Bei Auftragsverarbeitung: AVV als Vertragsbestandteil. Ergebnis: Software/Dienstleistung ist beschafft.*

**08 Implementieren und Berechtigungskonzept erstellen**  
*IT-Abteilung implementiert das Verfahren. Rechte- und Rollenkonzept (mindestens: Administrator, Fachanwender mit/ohne Schreibrechte, Auskunftsberechtigte, Einschränkungen) wird erstellt und dokumentiert. Schnittstellen zu anderen Systemen werden dokumentiert (System, Datenart, Übertragungsweg, Sicherheitsmaßnahmen).*

**09 Testen und Schulung durchführen**  
*Funktionstest, Berechtigungstest und Datenschutz-Prüfung (keine ungewollten Datenflüsse) unter praxisnahen Bedingungen. Nutzer werden vor Produktivbetrieb geschult (Bedienung, Datenschutz, Sicherheit, Verhalten bei Störungen). Schulungen dokumentieren. Informationspflichten nach Art. 13/14 DSGVO erfüllen.*

**10 Produktivsetzung und Dokumentation abschließen**  
*Produktivsetzung durch IT-Abteilung nach erfolgreichem Test und Freigabe. Abschließend zu dokumentieren und in der verantwortlichen Abteilung zu hinterlegen: VVT-Eintrag (Art. 30 DSGVO), Risikoanalyse (Art. 32 DSGVO), Berechtigungskonzept, Schnittstellen-Dokumentation, AVV (falls erforderlich), DSFA (falls erforderlich), Schulungsnachweise.*

**11 Regelmäßige Überprüfung**  
*Jährliche Prüfung: Sind Berechtigungen noch aktuell? Ist die DSFA noch gültig? Bestehen neue rechtliche Anforderungen? Sind Änderungen am Verfahren erforderlich? Bei wesentlichen Änderungen (neue Funktionen, neue Schnittstellen, neue Verarbeitungszwecke) ist der Prozess ab Phase 2 erneut zu durchlaufen und der Personalrat erneut zu beteiligen.*

---
*Dieser Entwurf wurde mit KI-Unterstützung erstellt. Inhaltliche Prüfung durch den Menschen erforderlich.*