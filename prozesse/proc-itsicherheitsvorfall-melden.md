---
id: proc-itsicherheitsvorfall-melden
titel: IT-Sicherheitsvorfall melden und erstbehandeln (Schadsoftware)
status: aktiv
zustaendigeEinheit: oe-amt-15
zustaendigeRolle: Sachbearbeitung
beteiligte:
  - einheit: oe-amt-1-5
    aufgabe: Bewertung des Sicherheitsvorfalls, forensische Analyse, Entscheidung über Eindämmungsmaßnahmen
  - einheit: oe-amt-1-4
    aufgabe: Prüfung auf Personenbezug, Auslösung des Data-Breach-Prozesses nach Art. 33/34 DSGVO
  - einheit: oe-hvb
    aufgabe: Entscheidung über Krisenstab und externe Kommunikation bei schwerwiegenden Vorfällen
daten:
  input:
    - Meldung der beschäftigten Person (Art des Vorfalls, betroffenes System, Zeitpunkt, beobachtete Symptome)
  output:
    - Ticket im Incident-Management-System, forensischer Bericht, ggf. Data-Breach-Meldung
  datenspeicher:
    - id: dstore-sicherheitsmangelmeldung
    - id: dstore-it-berechtigungsantrag
regelungen:
  - "BSI IT-Grundschutz (Incident Response)"
  - "NIST SP 800-61 Rev. 3 (Incident Response Lifecycle: Preparation → Detection → Containment/Eradication/Recovery → Post-Incident)"
  - "Art. 32 DSGVO (Sicherheit der Verarbeitung, TOM)"
  - "Art. 33 DSGVO (Meldepflicht bei Verletzung personenbezogener Daten)"
  - "Art. 5 Abs. 2 DSGVO (Rechenschaftspflicht, Dokumentation)"
  - "NIS-2-Richtlinie (EU 2022/2555) — Meldepflicht an BSI, soweit anwendbar"
  - "DA IT-Nutzung, DA Informationssicherheit"
leika_id: null
ozg_id: null
letzte-aktualisierung: '2026-08-23'
---
# IT-Sicherheitsvorfall melden und erstbehandeln (Schadsoftware)

## Zweck

Meldung und Erstbehandlung eines IT-Sicherheitsvorfalls durch eine beschäftigte Person — etwa bei Schadsoftware-Befall (Ransomware, Trojaner), Phishing mit erfolgreicher Anmeldung, unberechtigtem Zugriff oder verdächtigem Systemverhalten. Die beschäftigte Person meldet den Vorfall unverzüglich, leitet technische Sofortmaßnahmen ein (System vom Netz trennen) und übergibt an die IT-Abteilung und den ISB zur forensischen Analyse. Bei Personenbezug wird der Data-Breach-Prozess (`proc-data-breach`) ausgelöst.

**Anlaufstelle bei Sicherheitsvorfall:** IT-Abteilung (oe-amt-15) — telefonisch oder Ticketsystem. Bei Verdacht auf Datenverlust zusätzlich DSB (oe-amt-1-4) informieren.

## Prozessschritte

**01 Sicherheitsvorfall erkennen**
*Die beschäftigte Person bemerkt Anzeichen eines Sicherheitsvorfalls: ungewöhnliche Systemmeldungen (Ransomware-Hinweis, Pop-ups), plötzliche Verschlüsselung von Dateien, unerwartete Passwortänderungen, nicht autorisierte E-Mail-Aktivität, langsames oder abnormales Systemverhalten, unerklärliche Netzwerkaktivität.*

**02 System sofort trennen — keine eigenen Reparaturversuche**
*Die beschäftigte Person trennt das betroffene System unverzüglich vom Netzwerk: Netzwerkkabel ziehen, WLAN deaktivieren, das System nicht herunterfahren (flüchtige Beweise im Arbeitsspeicher bleiben erhalten). Keine eigenen Löschversuche, keine Virenscans, keine Neustarts — nach BSI-Checkliste „Ransomware: Erste Hilfe".*

**03 Meldung an die IT-Abteilung**
*Die beschäftigte Person meldet den Vorfall unverzüglich telefonisch oder über das Ticketsystem an die IT-Abteilung (oe-amt-15). Die Meldung umfasst: Art des Vorfalls (welche Anzeichen), betroffenes System (Rechnername, Standort), Zeitpunkt der Entdeckung, bereits ergriffene Maßnahmen. Die IT-Abteilung eröffnet ein Ticket im Incident-Management-System.*

**04 Bewertung durch den ISB**
*Die oder der Informationssicherheitsbeauftragte (oe-amt-1-5) bewertet den Vorfall nach NIST-Schema: Detection & Analysis — handelt es sich um einen Sicherheitsvorfall? Welcher Typ (Schadsoftware, unbefugter Zugriff, Phishing)? Welches Ausmaß (Einzelsystem, Netzwerksegment, gesamte Verwaltung)? Die Bewertung wird im Ticket dokumentiert.*

**05 Eindämmung, forensische Sicherung und Beseitigung**
*Der ISB veranlasst die Eindämmung (Containment): betroffene Systeme isolieren, Netzwerksegmente trennen, ggf. Firewall-Regeln anpassen. Eine forensische Sicherung wird durchgeführt (Arbeitsspeicher-Dump, Festplatten-Image, Logs exportieren). Anschließend erfolgt die Bereinigung (Eradication): Schadsoftware entfernen, Systeme neu aufsetzen. Die Wiederherstellung (Recovery) erfolgt aus geprüften Backups.*

**06 Prüfung auf Personenbezug und Data Breach**
*Die oder der Datenschutzbeauftragte (oe-amt-1-4) prüft, ob personenbezogene Daten betroffen sind. Ist dies der Fall, wird der Data-Breach-Prozess (`proc-data-breach`) ausgelöst: Meldung an die LfD Niedersachsen binnen 72 Stunden nach Art. 33 DSGVO, ggf. Betroffenenbenachrichtigung nach Art. 34 DSGVO.*

**07 Dokumentation und Lessons Learned**
*Der gesamte Vorfall wird dokumentiert: Zeitstrahl, ergriffene Maßnahmen, forensischer Bericht, Bewertung. Eine Nachbesprechung (Post-Incident Review nach NIST) identifiziert Schwachstellen und leitet Verbesserungen ab: TOM anpassen, Prozesse nachschärfen, ggf. Schulungen durchführen. Die Dokumentation dient der Rechenschaftspflicht nach Art. 5 Abs. 2 DSGVO.*

**Herkunft des Schrittblocks:** abgeleitet aus BSI-Checkliste IT-Sicherheitsvorfall, NIST SP 800-61 Rev. 3 (Incident Response Lifecycle), Art. 32/33 DSGVO sowie NIS-2-Richtlinie, nicht aus einer Ablauferhebung in der IT-Abteilung.