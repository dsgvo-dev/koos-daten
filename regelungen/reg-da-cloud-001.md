---
id: reg-da-001
name: Dienstanweisung zur Nutzung von Cloud-Diensten (DA Cloud)
typ: Dienstanweisung
status: aktiv
datum: '2023-03-15'
zustaendigeEinheit: oe-amt-1-5
entscheidendesGremium: Hauptverwaltungsbeamter
kontext: Die Verwaltung benötigt verbindliche Regelungen für den Einsatz von Cloud-Dienstleistungen.
entscheidung: Die DA Cloud gilt für alle Mitarbeitenden der Gemeindeverwaltung. Sie
  regelt den Einsatz von Cloud-Dienstleistungen im IT-Bereich. Insbesondere regelt
  sie, welche Daten mit welchem Schutzbedarf in Cloud-Lösungen eingestellt werden
  dürfen.
---

# **Dienstanweisung zur Nutzung von Cloud-Diensten in der [Name der Kommune]**

## **Geltungsbereich**
Diese Anweisung gilt für alle Mitarbeiter:innen der [Name der Kommune], einschließlich externer Dienstleister, die im Auftrag der Kommune Cloud-Dienste nutzen oder verwalten [1].

---

## **1. Grundsätze der Cloud-Nutzung**

### **1.1 Schutzbedarfsanalyse als Grundlage**
- Vor der Auslagerung von Daten in die Cloud ist eine **Schutzbedarfsanalyse** gemäß der IT-Sicherheitsrichtlinie der Kommune durchzuführen [1].
- Der Schutzbedarf bestimmt sich nach:
  - **Vertraulichkeit** (z. B. personenbezogene Daten, Sozialdaten, interne Verwaltungsvorgänge),
  - **Integrität** (z. B. Finanzdaten, Baupläne, behördliche Entscheidungen),
  - **Verfügbarkeit** (z. B. Notfallpläne, Bürgerdienste).

### **1.2 Datenkategorien und Cloud-Eignung**
Die Eignung von Daten für die Cloud-Nutzung richtet sich nach ihrem **Schutzbedarf** [1]:

| **Datenkategorie**                     | **Schutzbedarf**       | **Cloud-Nutzung**                     |
|----------------------------------------|------------------------|---------------------------------------|
| Öffentlich zugängliche Daten           | Kein Schutzbedarf      | Uneingeschränkt zulässig              |
| Dienstliche Daten (Verwaltung/Lehre)   | Hoch bis sehr hoch     | Nur mit Verschlüsselung und Genehmigung [1] |
| Sensible Daten (z. B. Sozialdaten, Gesundheitsdaten, Personalakten) | Sehr hoch | **Grundsätzlich unzulässig** [1]. Ausnahmen nur mit vorheriger Verschlüsselung unter Kontrolle der Kommune und schriftlicher Genehmigung der IT-Sicherheitsbeauftragten. |

---

## **2. Sicherheitsanforderungen an Cloud-Dienste**

### **2.1 Auswahl des Cloud-Anbieters**
- Der Anbieter muss **BSI-zertifiziert** sein (z. B. nach ISO 27001 oder BSI C5) [2].
- Es sind **deutsche oder EU-Rechenzentren** zu bevorzugen (DSGVO-konforme Datenverarbeitung).
- Der Anbieter muss **Transparenz über Speicherorte, Subunternehmer und Löschfristen** gewährleisten [1].

### **2.2 Verschlüsselung**
- Daten mit **hohem oder sehr hohem Schutzbedarf** sind **vor der Übertragung** zu verschlüsseln [1].
- Die Verschlüsselung muss **dem Stand der Technik entsprechen** (z. B. AES-256).
- **Schlüsselmanagement** obliegt ausschließlich der Kommune (z. B. durch das Rechenzentrum) [1].

### **2.3 Zugriffskontrollen**
- **Rollenbasierte Zugriffsrechte (RBAC)** sind verpflichtend.
- **Zwei-Faktor-Authentifizierung (2FA)** für alle Nutzer:innen.
- **Protokollierung aller Zugriffe** (Log-Daten mindestens 6 Monate speichern) [1].

### **2.4 Datenlöschung**
- Cloud-Anbieter müssen **sofortige Löschung** auf Anforderung garantieren.
- Bei **technisch bedingten Verzögerungen** ist dies vertraglich zu regeln und zu dokumentieren [1].

---

## **3. Genehmigungsverfahren**

### **3.1 Änderungen an Cloud-Diensten**
- Jede **Änderung der Datenverarbeitung in der Cloud** bedarf der **vorherigen Genehmigung** durch die IT-Sicherheitsbeauftragte und den Datenschutzbeauftragten [1].
- Die **Dokumentation der Schutzbedarfsanalyse** ist vorzulegen.

### **3.2 Ausnahmen für sensible Daten**
- Die Auslagerung von Daten mit **sehr hohem Schutzbedarf** ist nur in **absoluten Ausnahmefällen** zulässig [1].
- Die Entscheidung trifft die **Leitung der Kommune** nach Stellungnahme der IT-Sicherheitsbeauftragten.

---

## **4. Verantwortlichkeiten**

| **Rolle**                          | **Aufgaben**                                                                 |
|------------------------------------|------------------------------------------------------------------------------|
| **IT-Sicherheitsbeauftragte:r**    | Durchführung der Schutzbedarfsanalyse, Genehmigung von Cloud-Nutzungen [1]. |
| **Datenschutzbeauftragte:r**       | Prüfung der DSGVO-Konformität, Beratung bei sensiblen Daten.                |
| **Fachabteilungen**                | Einhaltung der Dienstanweisung, Meldung von Sicherheitsvorfällen.           |
| **Rechenzentrum**                  | Verwaltung der Verschlüsselung, Schlüsselmanagement [1].                    |

---

## **5. Schulung und Sensibilisierung**
- Alle Mitarbeiter:innen sind **jährlich** in den Sicherheitsrichtlinien für Cloud-Nutzung zu schulen.
- Besondere Schulungen für **Führungskräfte und IT-Verantwortliche** zu Schutzbedarfsanalysen und Verschlüsselung.

---

## **6. Sanktionen bei Verstößen**
- Verstöße gegen diese Anweisung können **disziplinarische Maßnahmen** nach sich ziehen.
- Bei **fahrlässiger oder vorsätzlicher Missachtung** drohen zivil- oder strafrechtliche Konsequenzen (z. B. nach DSGVO).

---

## **7. Inkrafttreten und Aktualisierung**
- Diese Anweisung tritt am **[Datum]** in Kraft.
- Sie wird **jährlich** überprüft und bei Bedarf angepasst [1].

---

## **Anlagen**
- **Anlage 1:** Vorlage für die Schutzbedarfsanalyse.
- **Anlage 2:** Checkliste für die Auswahl von Cloud-Anbietern.
- **Anlage 3:** Muster für die Genehmigungsanfrage.

# **Schutzbedarfsanalyse für Cloud-Nutzung**
**Verantwortliche Abteilung:** ________________________
**Datum:** ________________________

| **Kriterium**               | **Bewertung**                                                                 |
|-----------------------------|-------------------------------------------------------------------------------|
| **Datenkategorie**          | z. B. Personalakten, Sozialdaten, Baupläne, Bürgeranfragen                   |
| **Schutzbedarf**            | □ Normal □ Hoch □ Sehr hoch (Begründung: ______________________________) [1] |
| **Vertraulichkeit**         | □ Öffentlich □ Intern □ Vertraulich □ Geheim                                |
| **Integrität**              | □ Gering □ Mittel □ Hoch (z. B. "Baupläne müssen manipulationssicher sein") |
| **Verfügbarkeit**           | □ Gering (Toleranz: >24h) □ Mittel (Toleranz: <4h) □ Hoch (Toleranz: <1h)   |
| **Rechtliche Vorgaben**     | z. B. DSGVO, NDSG, SGB VIII, BSI-Grundschutz [1]                            |
| **Cloud-Eignung**           | □ Uneingeschränkt □ Mit Auflagen (z. B. Verschlüsselung) □ Unzulässig       |
| **Genehmigung erforderlich**| □ Ja □ Nein (Unterschrift IT-Sicherheitsbeauftragte: ______________________) |

**Hinweis:**
- Bei **hohem oder sehr hohem Schutzbedarf** ist eine **Risikoanalyse** durchzuführen [1].
- Die Vorlage ist **vor jeder Cloud-Nutzung** auszufüllen und zu dokumentieren.

# **Checkliste: Auswahl von Cloud-Dienstleistern**
**Anbieter:** ________________________
**Datum der Prüfung:** ________________________

| **Kriterium**                          | **Erfüllt?** (□ Ja □ Nein) | **Nachweis**                     |
|----------------------------------------|----------------------------|----------------------------------|
| **Zertifizierungen**                   |                            |                                  |
| - ISO 27001                            | □                          | Zertifikat vorlegen             |
| - BSI C5 (Cloud Computing Compliance)  | □                          | Zertifikat vorlegen [1]         |
| - ISO 27017 (Cloud-Sicherheit)         | □                          | Zertifikat vorlegen             |
| **Standort der Rechenzentren**         |                            |                                  |
| - EU/EWR (DSGVO-konform)               | □                          | Vertragliche Zusicherung        |
| - Keine Datenübermittlung in Drittländer | □                        | Vertragliche Zusicherung        |
| **Verschlüsselung**                    |                            |                                  |
| - Datenverschlüsselung (AES-256)       | □                          | Technische Spezifikation [1]    |
| - Schlüsselmanagement beim Kunden      | □                          | Vertragliche Regelung [1]       |
| **Zugriffskontrollen**                 |                            |                                  |
| - Rollenbasierte Zugriffe (RBAC)       | □                          | Dokumentation                    |
| - Zwei-Faktor-Authentifizierung (2FA)  | □                          | Technische Umsetzung             |
| **Datenlöschung**                      |                            |                                  |
| - Sofortige Löschung auf Anforderung   | □                          | Vertragliche Garantie [1]       |
| - Nachweisbare Löschung                | □                          | Protokollierung                  |
| **Auftragsverarbeitung (AV-Vertrag)**  |                            |                                  |
| - AV-Vertrag gemäß Art. 28 DSGVO       | □                          | Vertrag vorlegen [1]            |
| - Subunternehmer-Regelung              | □                          | Liste der Subunternehmer        |
| **Notfallmanagement**                  |                            |                                  |
| - Business-Continuity-Plan             | □                          | Dokumentation vorlegen          |
| - Wiederherstellungszeiten (RTO/RPO)   | □                          | Max. Ausfallzeit: _______       |

**Bewertung:**
- **Mindestens 80% der Kriterien müssen erfüllt sein** für die Zulassung.
- Bei **sensiblen Daten** (Schutzbedarf "sehr hoch") sind **alle Kriterien verpflichtend** [1].

# **Genehmigungsanfrage für Cloud-Nutzung**
**An:**
- IT-Sicherheitsbeauftragte:r
- Datenschutzbeauftragte:r

**Betreff:** Antrag auf Genehmigung der Cloud-Nutzung für ________________________

### **1. Antragsteller**
- **Name:** ________________________
- **Abteilung:** ________________________
- **Kontaktdaten:** ________________________

### **2. Beschreibung des Cloud-Dienstes**
- **Anbieter:** ________________________
- **Zweck der Nutzung:** ________________________
- **Geplante Datenkategorien:** ________________________
- **Schutzbedarf:** □ Normal □ Hoch □ Sehr hoch (gemäß Anlage 1) [1]

### **3. Sicherheitsmaßnahmen**
- **Verschlüsselung:** □ Ja (Methode: _______) □ Nein
- **Zugriffskontrollen:** □ RBAC □ 2FA □ Sonstiges: _______
- **AV-Vertrag:** □ Vorhanden (Anlage) □ Fehlt [1]

### **4. Schutzbedarfsanalyse & Risikoanalyse**
- **Anlage 1 (Schutzbedarfsanalyse) beigefügt:** □ Ja □ Nein
- **Risikoanalyse durchgeführt:** □ Ja □ Nein (bei "sehr hohem" Schutzbedarf) [1]

### **5. Erklärung**
Hiermit bestätige ich, dass die Angaben vollständig und korrekt sind. Ich verpflichte mich zur Einhaltung der Dienstanweisung zur Cloud-Nutzung.

**Datum:** ___________ **Unterschrift:** _______________________

### **6. Entscheidung**
- **IT-Sicherheitsbeauftragte:r:**
  □ Genehmigt □ Genehmigt mit Auflagen: ________________________ □ Abgelehnt
  **Datum:** ___________ **Unterschrift:** _______________________

**Hinweis:**
- Die Bearbeitung dauert **max. 10 Werktage**.
- Bei **sensiblen Daten** ist zusätzlich die **Genehmigung der Verwaltungsleitung** erforderlich [1].

# **Auftragsverarbeitungsvertrag (AV-Vertrag) gemäß Art. 28 DSGVO**
**Zwischen:**
[Name der Kommune], vertreten durch ________________________
– **nachfolgend "Auftraggeber"** –

**und:**
[Name des Cloud-Anbieters], vertreten durch ________________________
– **nachfolgend "Auftragnehmer"** –

### **§ 1 Gegenstand und Dauer**
1. Der Auftragnehmer verarbeitet personenbezogene Daten im Auftrag des Auftraggebers gemäß den Weisungen des Auftraggebers.
2. Die Verarbeitung erfolgt ausschließlich für die in **Anlage 1** beschriebenen Zwecke.

### **§ 2 Technische und organisatorische Maßnahmen (TOM)**
Der Auftragnehmer gewährleistet folgende Maßnahmen:
- Verschlüsselung der Daten (AES-256) [1].
- Zugriff nur für autorisierte Personen (RBAC + 2FA).
- Protokollierung aller Zugriffe (Log-Daten für 6 Monate).
- Regelmäßige Sicherheitsaudits (mind. jährlich).

### **§ 3 Unterauftragsverarbeiter**
1. Der Auftragnehmer darf Subunternehmer nur mit vorheriger schriftlicher Zustimmung des Auftraggebers einsetzen.
2. Eine Liste aller Subunternehmer ist als **Anlage 2** beizufügen.

### **§ 4 Datenlöschung und Beendigung**
1. Der Auftragnehmer löscht alle Daten nach Beendigung des Vertrags **unverzüglich** [1].
2. Eine Bestätigung der Löschung ist dem Auftraggeber vorzulegen.

### **§ 5 Haftung und Schadensersatz**
1. Der Auftragnehmer haftet für Schäden, die durch Verstöße gegen diesen Vertrag entstehen.
2. Der Auftraggeber ist berechtigt, den Vertrag fristlos zu kündigen, wenn der Auftragnehmer gegen wesentliche Pflichten verstößt.

### **§ 6 Schlussbestimmungen**
1. Änderungen bedürfen der **Schriftform**.
2. Gerichtsstand ist der Sitz des **Auftraggebers**.

**Anlagen:**
- Anlage 1: Beschreibung der Verarbeitungszwecke.
- Anlage 2: Technische und organisatorische Maßnahmen (TOM).
- Anlage 3: Liste der Subunternehmer.

# **Cloud-Register der [Name der Kommune]**
**Stand:** ________________________

| **Cloud-Dienst**       | **Anbieter**       | **Datenkategorie**       | **Schutzbedarf** | **AV-Vertrag** | **Genehmigung** | **Verantwortliche Abteilung** | **Letzte Prüfung** |
|------------------------|--------------------|--------------------------|------------------|----------------|-----------------|-------------------------------|--------------------|
| z. B. Microsoft 365    | Microsoft          | E-Mails, Kalender        | Hoch             | Ja [1]         | 15.03.2024      | Hauptamt                      | 01.06.2024         |
| z. B. Nextcloud        | Eigenbetrieb       | Bürgerdaten (Formulare)  | Normal           | Nein           | 10.01.2024      | Bürgerbüro                    | 01.06.2024         |

**Hinweis:**
- Das Register wird **vierteljährlich** von der IT-Sicherheitsbeauftragten überprüft.
- Bei **Verstößen** gegen die Dienstanweisung wird der Dienst **sofort gesperrt** [1].