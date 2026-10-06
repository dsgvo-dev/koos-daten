---
id: proc-telefonie-einrichten-und-betreiben
titel: Telekommunikationsanlage einrichten und betreiben
typ: Prozess
status: aktiv
bereich: intern
zustaendigeEinheit: oe-amt-15
beteiligte:
  - einheit: oe-amt-1-4
    aufgabe: >-
      Einsicht in die Dokumentation (Schritt 08; DV § 10 Abs. 1);
      Kontrollinstanz mit Zugriff auf gespeicherte Daten (DV § 9 Abs. 2
      lit. d); Auskunftsersuchen der Beschäftigten (DV § 11 Abs. 1)
  - einheit: oe-personalrat
    aufgabe: >-
      Mitbestimmung nach § 78 NPersVG, Abschluss DV (Schritt 01);
      Abstimmung Leistungsmerkmale (Schritt 02); Information vor
      Stichproben (Schritt 06); Zustimmung zu technischen Änderungen
      (Schritt 07); jährliche Überprüfung der Einhaltung der DV
      (Schritt 08)
  - einheit: oe-amt-15
    aufgabe: >-
      Amtsberechtigungen vergeben, Sonderanschlüsse für PR/DSB/SBV
      einrichten (Schritt 03); Verfahrensbeschreibung pflegen
      (DV § 10 Abs. 1); Wartung (DV § 10 Abs. 2); Zugriff für Betrieb,
      Wartung und Störungsbeseitigung (DV § 9 Abs. 2 lit. b);
      Gebührenabrechnung nach Kostenstellen, Löschung der
      Verbindungsdaten, Protokollierung der Zugriffe, Backup
      (Schritt 05; DV § 10 Abs. 4)
  - rolle: Telefonzentrale
    phase: "5,6"
    aufgabe: >-
      Teilnehmerverzeichnis pflegen, Freischaltungsanträge für
      Sonderrufnummern bearbeiten (Schritt 05; DV § 6 Abs. 3);
      Einzelverbindungsnachweise auf Antrag (Schritt 06); Aufschalten
      auf laufende Gespräche (DV § 3 Abs. 5)
daten:
  input:
    - >-
      Stammdaten der Beschäftigten (Name, Vorname, Nebenstellennummer,
      Kostenstelle)
    - >-
      Verbindungsdaten (dienstlich): Zielrufnummer, Datum, Uhrzeit,
      Dauer, Gebühreneinheiten
  output:
    - Teilnehmerverzeichnis (gepflegt durch Telefonzentrale)
    - Monatliche Gebührenabrechnung nach Kostenstellen
    - Zugriffsprotokolle (Administration)
    - Einzelverbindungsnachweise (auf Antrag)
  datenspeicher:
    - id: dstore-tk-teilnehmerdaten
    - id: dstore-tk-verbindungsdaten
    - id: dstore-tk-voicemail
regelungen:
  - reg-dv-telefonie - Dienstvereinbarung nach § 78 NPersVG
  - § 67 Abs. 1 Nr. 2 NPersVG - Mitbestimmung technische Einrichtungen
  - § 3 TDDDG - Fernmeldegeheimnis
  - Art. 88 DSGVO i.V.m. § 12 NDSG - Beschäftigtendatenschutz
letzte-aktualisierung: 2026-09-30
---

# Telekommunikationsanlage einrichten und betreiben

**01 Grundlage in der Dienstvereinbarung schaffen**
*Die Dienstvereinbarung Telekommunikationsanlagen (`reg-dv-telefonie`) nach § 78 NPersVG regelt Zweck, Umfang, Nutzungsbedingungen, Zugriffsberechtigungen, private Nutzung, Abrechnung und Löschfristen. Sie ist zugleich Kollektivvereinbarung im Sinne des Art. 88 DSGVO. Die Telekommunikationsanlage ist nach § 67 Abs. 1 Nr. 2 NPersVG mitbestimmungspflichtig.*

**02 Leistungsmerkmale festlegen und dokumentieren**
*In Abstimmung mit dem Personalrat werden die zentral bereitgestellten und gruppenspezifischen Leistungsmerkmale (Anlage 1 zur DV) festgelegt und in der Verfahrensbeschreibung dokumentiert. Dazu gehören: Identifizieren, Freisprechen, Rückruf, Anrufumleitung, Konferenz, Voice-Mail, Rufnummernanzeige, Chef-Sekretärfunktion. Änderungen unterliegen der erneuten Mitbestimmung.*

**03 Berechtigungskonzept einrichten**
*Für jeden Telefonanschluss werden durch die IT-Administration Amtsberechtigungen vergeben (keine, Nahbereich, Fernbereich deutschlandweit, Ausland). Sonderrufnummern (018xx, 0190x) sind standardmäßig gesperrt. Es ist keine Privattelefonie erlaubt. Sonderanschlüsse für Personalrat, Schwerbehindertenvertretung und Datenschutzbeauftragten werden ohne Einzelverbindungsdatenspeicherung eingerichtet.*

**04 Beschäftigte informieren und verpflichten**
*Bei Inkrafttreten der DV werden alle Beschäftigten per Rundschreiben über ihre Rechte und Pflichten informiert. Die Kenntnisnahme ist aktenkundig festzuhalten. IT-Administratoren und Beschäftigte der Telefonzentrale werden auf das Datengeheimnis und das Fernmeldegeheimnis (§ 3 TDDDG) verpflichtet. Die Verpflichtung wird dokumentiert.*

**05 Nutzung betreiben und überwachen**
*Den laufenden Betrieb führt die IT-Administration durch: monatliche Gebührenabrechnung (dienstlich nach Kostenstellen), Löschung der Verbindungsdaten nach Fristablauf (3 Monate), Protokollierung jedes Datenzugriffs, regelmäßige Datensicherung (Backup). Die Telefonzentrale pflegt das Teilnehmerverzeichnis und bearbeitet Freischaltungsanträge für Sonderrufnummern.*

**06 Kontrolle und Stichproben**
*Stichproben zur Überprüfung auf missbräuchliche Nutzung sind nur nach vorheriger Information des Personalrats durch die Dienststellenleitung zulässig. Verbindungsdaten werden nach dem Zufallsprinzip ausgewählter Nebenstellen ausgedruckt und nach Auswertung gelöscht. Einzelverbindungsnachweise können durch die Einrichtungsleitung formlos bei der Telefonzentrale beantragt werden.*

**07 Änderungen und Erweiterungen durchführen**
*Jede technische Änderung, die den Datenschutz berührt (Hardware, Software, Leistungsmerkmale), ist dem Personalrat rechtzeitig mitzuteilen und bedarf dessen Zustimmung. Release- und Versionswechsel werden dokumentiert. Die Verfahrensbeschreibung und Anlage 1 zur DV sind fortzuschreiben.*

**08 Jährliche Überprüfung**
*Dienststelle und Personalrat überprüfen jährlich die Einhaltung der DV. Der Datenschutzbeauftragte erhält Einsicht in die Dokumentation. Wesentliche Änderungen der Telekommunikationsinfrastruktur (z. B. Migration zu VoIP) werden im Rahmen eines neuen Mitbestimmungsverfahrens behandelt.*
