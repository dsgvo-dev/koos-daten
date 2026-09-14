---
id: reg-da-cloud
name: Dienstanweisung zur Nutzung von Cloud-Diensten (DA Cloud)
typ: Dienstanweisung
status: aktiv
datum: '2023-09-14'
zustaendigeEinheit: oe-amt-1-5
entscheidendes-gremium: Hauptverwaltungsbeamter
---

# **Dienstanweisung zur Nutzung von Cloud-Diensten in der [Musterkommune]**

## **Geltungsbereich**
Diese Anweisung gilt für alle Mitarbeiter:innen der [Musterkommune], einschließlich externer Dienstleister, die im Auftrag der Kommune Cloud-Dienste nutzen oder verwalten.

---

## **1. Grundsätze der Cloud-Nutzung**

### **1.1 Schutzbedarfsanalyse als Grundlage**
- Vor der Auslagerung von Daten in die Cloud ist eine **Schutzbedarfsanalyse** gemäß der IT-Sicherheitsrichtlinie der Kommune durchzuführen.
- Der Schutzbedarf bestimmt sich nach:
  - **Vertraulichkeit** (z. B. personenbezogene Daten, Sozialdaten, interne Verwaltungsvorgänge),
  - **Integrität** (z. B. Finanzdaten, Baupläne, behördliche Entscheidungen),
  - **Verfügbarkeit** (z. B. Notfallpläne, Bürgerdienste).

### **1.2 Datenkategorien und Cloud-Eignung**

Die Eignung von Daten für die Cloud-Nutzung richtet sich nach dem **Schutzbedarf**
gemäß der Richtlinie zur Datenklassifizierung. Deren
Anlage B (Umgangsmatrix) legt in der Zeile „**Cloud-Speicher**" für jede
Kombination aus Datenschutz-Schutzstufe (A–E) und Vertraulichkeitsstufe (V1–V4)
fest, ob und unter welchen Bedingungen eine Cloud-Nutzung zulässig ist:

- V1 / A — beliebig zulässig.
- V2 / B — nur in vom ISB freigegebenen EU-Diensten.
- V3 / C–D — nur freigegebene EU-Dienste + zusätzliche Verschlüsselung unter
  Kontrolle der Verwaltung.
- V4 / E — nicht zulässig außer mit Einzelgenehmigung der Verwaltungsleitung
  nach ISB-Stellungnahme.

Die Schutzbedarfsanalyse (§ 1.1) und die Anbieterauswahl (§ 2) setzen auf
diesen Vorgaben auf. Bei Unsicherheit über
die Einstufung einer Datenart ist die/der ISB hinzuzuziehen.

---

## **2. Sicherheitsanforderungen an Cloud-Dienste**

### **2.1 Auswahl des Cloud-Anbieters**
- Der Anbieter muss **BSI-zertifiziert** sein (z. B. nach ISO 27001 oder BSI C5).
- Es sind **deutsche oder EU-Rechenzentren** zu bevorzugen (DSGVO-konforme Datenverarbeitung).
- Der Anbieter muss **Transparenz über Speicherorte, Subunternehmer und Löschfristen** gewährleisten.

### **2.2 Verschlüsselung**
- Daten mit **hohem oder sehr hohem Schutzbedarf** sind **vor der Übertragung** zu verschlüsseln.
- Die Verschlüsselung muss **dem Stand der Technik entsprechen** (z. B. AES-256).
- **Schlüsselmanagement** obliegt ausschließlich der Kommune (z. B. durch das Rechenzentrum).

### **2.3 Zugriffskontrollen**
- **Rollenbasierte Zugriffsrechte (RBAC)** sind verpflichtend.
- **Zwei-Faktor-Authentifizierung (2FA)** für alle Nutzer:innen.
- **Protokollierung aller Zugriffe** (Log-Daten mindestens 6 Monate speichern).

### **2.4 Datenlöschung**
- Cloud-Anbieter müssen **sofortige Löschung** auf Anforderung garantieren.
- Bei **technisch bedingten Verzögerungen** ist dies vertraglich zu regeln und zu dokumentieren.

---

## **3. Genehmigungsverfahren**

### **3.1 Änderungen an Cloud-Diensten**
- Jede **Änderung der Datenverarbeitung in der Cloud** bedarf der **vorherigen Genehmigung** durch die IT-Sicherheitsbeauftragte und den Datenschutzbeauftragten.
- Die **Dokumentation der Schutzbedarfsanalyse** ist vorzulegen.

### **3.2 Ausnahmen für sensible Daten**
- Die Auslagerung von Daten mit **sehr hohem Schutzbedarf** ist nur in **absoluten Ausnahmefällen** zulässig.
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
- Bei **fahrlässiger oder vorsätzlicher Missachtung** drohen zivil- oder strafrechtliche Konsequenzen.

---

## **7. Inkrafttreten und Aktualisierung**
- Diese Anweisung tritt am **[Datum]** in Kraft.
- Sie wird **jährlich** überprüft und bei Bedarf angepasst.

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
- Bei **hohem oder sehr hohem Schutzbedarf** ist eine **Risikoanalyse** durchzuführen.
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
| **Auftragsverarbeitung**  |                            |                                  |
| - AV-Vertrag (Art. 28 DSGVO)       | □                          | Vertrag nach AVV-Muster vorlegen — das Muster liegt bei der Rechtsabteilung (nicht Teil dieser DA) |
| **Notfallmanagement**                  |                            |                                  |
| - Business-Continuity-Plan             | □                          | Dokumentation vorlegen          |
| - Wiederherstellungszeiten (RTO/RPO)   | □                          | Max. Ausfallzeit: _______       |

**Bewertung:**
- **Mindestens 80% der Kriterien müssen erfüllt sein** für die Zulassung.
- Bei **sensiblen Daten** (Schutzbedarf "sehr hoch") sind **alle Kriterien verpflichtend**.

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
- **Schutzbedarf:** □ Normal □ Hoch □ Sehr hoch (gemäß Anlage 1)

### **3. Sicherheitsmaßnahmen**
- **Verschlüsselung:** □ Ja (Methode: _______) □ Nein
- **Zugriffskontrollen:** □ RBAC □ 2FA □ Sonstiges: _______
- **AV-Vertrag:** □ Vorhanden (nach AVV-Muster der Rechtsabteilung — Anlage) □ Fehlt

### **4. Schutzbedarfsanalyse & Risikoanalyse**
- **Anlage 1 (Schutzbedarfsanalyse) beigefügt:** □ Ja □ Nein
- **Risikoanalyse durchgeführt:** □ Ja □ Nein (bei "sehr hohem" Schutzbedarf)

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

## **8. Auftragsverarbeitung (AV-Vertrag nach Art. 28 DSGVO)**

Der Abschluss eines Auftragsverarbeitungsvertrags ist **Pflicht**, bevor
personenbezogene Daten in eine Cloud ausgelagert werden. Das AVV-Muster liegt
bei der Rechtsabteilung und ist nicht Teil dieser DA — es wird bei Bedarf
angefordert.

Die **Checkliste für die Auswahl von Cloud-Dienstleistern** (Abschnitt 7)
fragt den AV-Vertrag als Einzelkriterium ab; der Vertrag selbst wird nach dem
Muster der Rechtsabteilung geschlossen.

---

## **9. Cloud-Register der [Musterkommune]**
**Stand:** ________________________

| **Cloud-Dienst**       | **Anbieter**       | **Datenkategorie**       | **Schutzbedarf** | **Genehmigung** | **Verantwortliche Abteilung** | **Letzte Prüfung** |
|------------------------|--------------------|--------------------------|------------------|-----------------|-------------------------------|--------------------|
| z. B. Microsoft 365    | Microsoft          | E-Mails, Kalender        | Hoch             | 15.03.2024      | Hauptamt                      | 01.06.2024         |
| z. B. Nextcloud        | Eigenbetrieb       | Bürgerdaten (Formulare)  | Normal           | 10.01.2024      | Bürgerbüro                    | 01.06.2024         |

**Hinweis:**
- Das Register wird **vierteljährlich** von der IT-Sicherheitsbeauftragten überprüft.
- Bei **Verstößen** gegen die Dienstanweisung wird der Dienst **sofort gesperrt**.
