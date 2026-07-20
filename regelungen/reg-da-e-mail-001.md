---
id: reg-da-e-mail-001
name: Dienstanweisung zur Nutzung von E-Mails (DA E-Mail)
typ: Dienstanweisung
status: aktiv
datum: '2023-03-15'
zustaendigeEinheit: oe-amt-15
entscheidendesGremium: Hauptverwaltungsbeamter
kontext: Die Verwaltung benötigt verbindliche Regelungen für den Einsatz von E-Mail-Diensten.
entscheidung: Die DA E-Mail gilt für alle Mitarbeitenden der Gemeindeverwaltung. Sie
  regelt den Einsatz von E-Mail-Diensten. Insbesondere regelt sie, welche Daten mit
  welchem Schutzbedarf per E-Mail versendet werden dürfen.
---

### **Dienstanweisung zur Nutzung von E-Mails in der [Name der Kommune] (DA E-Mail)**
**Gültig ab:** [Datum]
**Verantwortlich:** IT-Sicherheitsbeauftragter / Hauptamt
**Ersetzt:** [ggf. vorherige Version]

---

#### **1. Zweck und Geltungsbereich**
Diese Dienstanweisung regelt die **sichere und rechtskonforme Nutzung von E-Mails** für alle Beschäftigten der [Name der Kommune], einschließlich Auszubildender, Praktikant:innen und externer Dienstleister:innen mit Zugriff auf das kommunale E-Mail-System. Sie gilt für **dienstliche E-Mails** innerhalb und außerhalb des kommunalen Netzwerks und orientiert sich an:

* den **Vorgaben des BSI** (insbesondere BSI-Grundschutz, IT-Grundschutz-Kompendium),
* den **Datenschutzbestimmungen** (DSGVO, NDSG, BDSG),
* den **hausinternen Richtlinien** zur Informationssicherheit (*Allgemeine Gesc...5.2025.pdf*),
* den **Dienstvereinbarungen** zur Nutzung elektronischer Post (*allgemeine_dien...19 (1).pdf*).

**Ausnahmen** bedürfen der schriftlichen Genehmigung durch die IT-Leitung oder den Datenschutzbeauftragten.

---

#### **2. Grundsätze der E-Mail-Nutzung**
##### **2.1 Dienstliche Nutzung**
E-Mails dürfen **ausschließlich für dienstliche Zwecke** versendet werden. Private Nutzung ist untersagt (*Allgemeine Gesc...5.2025.pdf*).

##### **2.2 Vorrang vor Postversand**
Elektronische Kommunikation ist **grundsätzlich dem Postversand vorzuziehen**, sofern keine gesetzlichen oder vertraglichen Einschränkungen (z. B. Schriftformerfordernis) entgegenstehen (*Allgemeine Gesc...5.2025.pdf*).

##### **2.3 Gleichstellung mit Schriftverkehr**
E-Mails mit **qualifizierter elektronischer Signatur (QES)** oder **De-Mails** (absenderbestätigt) stehen schriftlichen Dokumenten gleich (*allgemeine_dien...19 (1).pdf*). Dies gilt insbesondere für:
* Bescheide,
* Verträge,
* Widersprüche,
* Mitteilungen an Gerichte, Staatsanwaltschaften oder andere Behörden.

##### **2.4 Verbot der Nutzung privater E-Mail-Konten**
Dienstliche E-Mails dürfen **nicht über private Konten** (z. B. Gmail, Web.de) versendet oder empfangen werden.

---

#### **3. Schutzbedarf und Verschlüsselungspflichten**
Die Kommune klassifiziert E-Mails nach **Schutzstufen** (niedrig, normal, hoch, sehr hoch). **Datenschutzrelevante, personenbezogene oder vertrauliche Informationen dürfen nicht per E-Mail übertragen werden** – weder im Inhalt noch in Anhängen (*Allgemeine Gesc...5.2025.pdf*). Ausnahmen:
* **Ende-zu-Ende-Verschlüsselung** (z. B. S/MIME, PGP) oder
* **De-Mail mit QES** für Behördenkommunikation (*allgemeine_dien...19 (1).pdf*).

| **Schutzstufe** | **Beispiele für Inhalte**                     | **Zulässige Übertragungsart**                     | **Empfängerkreis**                     |
|-----------------|-----------------------------------------------|---------------------------------------------------|----------------------------------------|
| **Niedrig**     | Allgemeine Anfragen, öffentliche Bekanntmachungen | Unverschlüsselt (TLS empfohlen)                   | Alle                                   |
| **Normal**      | Interne Mitteilungen                           | Transportverschlüsselung (TLS)                    | Behörden, Unternehmen                  |
| **Hoch**        | Personenbezogene Daten (z. B. Adressen)        | Ende-zu-Ende-Verschlüsselung oder De-Mail         | Behörden, Gerichte                     |
| **Sehr hoch**   | Gesundheitsdaten, Jugendamtsakten             | Nur über sichere Behördenpostfächer (z. B. EGVP)  | **Ausschließlich** Behörden/Gerichte   |

**Hinweis:**
* **Sozialdaten** (§ 67 SGB X) erfordern **immer** eine Ende-zu-Ende-Verschlüsselung oder De-Mail.
* **Daten mit sehr hohem Schutzbedarf** (z. B. Strafverfolgungsdaten) dürfen **nicht per E-Mail** versendet werden (*Allgemeine Gesc...5.2025.pdf*).

---

#### **4. Technische und organisatorische Maßnahmen (TOM)**
##### **4.1 Verschlüsselung**
* **Transportverschlüsselung (TLS):** Standardmäßig aktiviert.
* **Ende-zu-Ende-Verschlüsselung:** Für E-Mails mit hohem Schutzbedarf (Zertifikate durch IT bereitgestellt).
* **De-Mail:** Für rechtsverbindliche Kommunikation mit Behörden (*allgemeine_dien...19 (1).pdf*).

##### **4.2 Authentifizierung**
* **Zwei-Faktor-Authentifizierung (2FA)** für E-Mail-Zugriff.
* **Passwortrichtlinien:** Mindestens 12 Zeichen, Wechsel alle 90 Tage.

##### **4.3 E-Mail-Signatur**
Alle ausgehenden E-Mails müssen eine **standardisierte Signatur** mit folgenden Angaben enthalten:
* Name, Dienststelle, Telefonnummer,
* Rechtlicher Hinweis (z. B. *"Vertraulich – nur für den Adressaten"*),
* Link zur Datenschutzerklärung.

##### **4.4 Protokollierung und Archivierung**
* E-Mails mit **hohem/sehr hohem Schutzbedarf** werden **10 Jahre archiviert**.
* **Protokollierung** von Zugriffen (gemäß § 64 NDSG).

##### **4.5 Verbot von Massenmails**
* **Newsletter/Rundmails** an Externe bedürfen der Genehmigung durch die Pressestelle.

---

#### **5. Umgang mit sensiblen Daten**
##### **5.1 Verbotene Inhalte**
Folgende Daten dürfen **niemals per E-Mail** versendet werden:
* Passwörter, Zugangsdaten, Bankverbindungen,
* Daten mit **sehr hohem Schutzbedarf** (z. B. Jugendamtsakten) (*Allgemeine Gesc...5.2025.pdf*).

##### **5.2 Anlagen**
* **Passwortgeschützte Anhänge** (Passwort separat übermitteln).
* **Maximale Dateigröße:** 20 MB (größere Dateien über gesicherte File-Transfer-Systeme).

##### **5.3 Empfangsbestätigungen**
* Bei E-Mails mit **hohem Schutzbedarf** ist eine **Lesebestätigung** anzufordern.

---

#### **6. Verhalten bei Sicherheitsvorfällen**
##### **6.1 Datenpanne**
1. **Sofortige Meldung** an Datenschutzbeauftragten und IT-Sicherheit.
2. **Rückruf der E-Mail** (falls möglich).
3. **Dokumentation** (gemäß Art. 33 DSGVO).

##### **6.2 Phishing/Malware**
* **Keine Anhänge/Links** aus unbekannten Quellen öffnen.
* Verdächtige E-Mails an **it-sicherheit@[kommune].de** weiterleiten.

---

#### **7. Schulung und Verantwortlichkeiten**
##### **7.1 Schulungen**
* **Jährliche Schulung** für alle Beschäftigten.
* **Einweisung** für neue Mitarbeiter:innen vor Tätigkeitsaufnahme.

##### **7.2 Verantwortlichkeiten**
* **IT-Abteilung:** Bereitstellung sicherer Systeme, Zertifikatsverwaltung.
* **Fachbereiche:** Klassifizierung von E-Mails nach Schutzbedarf.
* **Datenschutzbeauftragter:** Überwachung der Einhaltung.

---

#### **8. Inkrafttreten und Überprüfung**
* **Inkrafttreten:** [Datum]
* **Jährliche Überprüfung** durch die IT-Sicherheit.

**Unterschrift:**
[Name], [Position]
[Name der Kommune], [Datum]

---

### **Anlagen**
1. Schutzstufenklassifizierung (BSI-Grundschutz)
2. Muster-E-Mail-Signatur
3. Liste sicherer Behördenpostfächer (EGVP, OSCI)
4. Verfahrensanweisung bei Datenpannen