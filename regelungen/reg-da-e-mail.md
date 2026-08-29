---
id: reg-da-e-mail
name: Dienstanweisung zur Nutzung von E-Mails (DA E-Mail)
typ: Dienstanweisung
status: entwurf
datum: '2023-03-15'
zustaendigeEinheit: oe-amt-15
entscheidendes-gremium: Hauptverwaltungsbeamter
---

# Dienstanweisung zur Nutzung von E-Mails in der [Name der Kommune] (DA E-Mail)
**Gültig ab:** [Datum]
**Verantwortlich:** IT-Sicherheitsbeauftragter / Hauptamt
**Ersetzt:** [ggf. vorherige Version]

---

## § 1 Zweck und Geltungsbereich
(1) Diese Dienstanweisung regelt die sichere und rechtskonforme Nutzung von E-Mails.

(2) Sie gilt für alle Beschäftigten der [Name der Kommune], einschließlich Auszubildender, Praktikantinnen und Praktikanten sowie externer Dienstleisterinnen und Dienstleister mit Zugriff auf das kommunale E-Mail-System.

(3) Sie gilt für dienstliche E-Mails innerhalb und außerhalb des kommunalen Netzwerks.

(4) Sie orientiert sich an:

* den **Vorgaben des BSI** (insbesondere BSI-Grundschutz, IT-Grundschutz-Kompendium),
* den **Datenschutzbestimmungen** (DSGVO, NDSG, BDSG),
* der **Informationssicherheitsleitlinie** (`reg-isl`),
* der **Dienstvereinbarung zur Nutzung elektronischer Post** [Fundstelle ergänzen].

(5) Ausnahmen von dieser Dienstanweisung bedürfen der schriftlichen Genehmigung durch die IT-Leitung oder die Datenschutzbeauftragte oder den Datenschutzbeauftragten.

---

## § 2 Grundsätze der E-Mail-Nutzung
### § 2.1 Dienstliche Nutzung
(1) E-Mails dürfen ausschließlich für dienstliche Zwecke versendet werden.

(2) Die private Nutzung des dienstlichen E-Mail-Systems ist untersagt.

### § 2.2 Vorrang vor Postversand
(1) Elektronische Kommunikation ist dem Postversand grundsätzlich vorzuziehen.

(2) Absatz 1 gilt nicht, soweit gesetzliche oder vertragliche Einschränkungen entgegenstehen, insbesondere ein Schriftformerfordernis.

### § 2.3 Gleichstellung mit Schriftverkehr
(1) E-Mails mit qualifizierter elektronischer Signatur (QES) und absenderbestätigte De-Mails stehen schriftlichen Dokumenten gleich.

(2) Absatz 1 gilt insbesondere für:
* Bescheide,
* Verträge,
* Widersprüche,
* Mitteilungen an Gerichte, Staatsanwaltschaften oder andere Behörden.

### § 2.4 Verbot der Nutzung privater E-Mail-Konten
(1) Dienstliche E-Mails dürfen nicht über private Konten versendet oder empfangen werden.

(2) Als private Konten gelten insbesondere Postfächer bei frei zugänglichen Anbietern.

---

## § 3 Schutzbedarf und Verschlüsselungspflichten
(1) Die Einstufung richtet sich nach der Richtlinie zur Datenklassifizierung (`reg-klassifizierung`). Maßgeblich sind die dort festgelegten Schutzstufen A–E und Vertraulichkeitsklassen V1–V4.

(2) Anlage B der Richtlinie enthält die Umgangsmatrix; deren Zeile „Übermittlung E-Mail" füllt dieser Paragraph aus.

(3) Datenschutzrelevante, personenbezogene oder vertrauliche Informationen dürfen nicht unverschlüsselt per E-Mail übertragen werden, weder im Inhalt noch in Anhängen. Zulässig sind:
* **Ende-zu-Ende-Verschlüsselung** (z. B. S/MIME, PGP) oder
* **De-Mail mit QES** für Behördenkommunikation.

(4) Für die Übermittlung gilt:

| **Stufe (V / A–E)** | **Beispiele für Inhalte** | **Zulässige Übertragungsart** | **Empfängerkreis** |
|-----------------|-----------------------------------------------|---------------------------------------------------|----------------------------------------|
| **V1 / A — Öffentlich** | Allgemeine Anfragen, öffentliche Bekanntmachungen | Unverschlüsselt (TLS empfohlen) | Alle |
| **V2 / B — Intern** | Interne Mitteilungen | Transportverschlüsselung (TLS) | Behörden, Unternehmen |
| **V3 / C–D — Vertraulich** | Personenbezogene Daten (z. B. Adressen) | Ende-zu-Ende-Verschlüsselung (S/MIME, PGP) oder De-Mail mit QES | Behörden, Gerichte |
| **V4 / E — Streng vertraulich** | Gesundheitsdaten, Jugendamtsakten | Nur über sichere Behördenpostfächer (EGVP, OSCI); **keine E-Mail** | **Ausschließlich** Behörden/Gerichte |

(5) Sozialdaten im Sinne des § 67 SGB X erfordern stets eine Ende-zu-Ende-Verschlüsselung oder De-Mail.

(6) Daten der Stufen V4 / E, insbesondere Strafverfolgungsdaten, dürfen nicht per E-Mail versendet werden.

---

## § 4 Technische und organisatorische Maßnahmen
### § 4.1 Verschlüsselung
(1) Es gelten folgende Verfahren:

* **Transportverschlüsselung (TLS):** Standardmäßig aktiviert.
* **Ende-zu-Ende-Verschlüsselung:** Für E-Mails der Stufen **V3 / C–D** aufwärts (Zertifikate durch IT bereitgestellt).
* **De-Mail:** Für rechtsverbindliche Kommunikation mit Behörden.

### § 4.2 Authentifizierung
(1) Der Zugriff auf das E-Mail-System erfordert eine Zwei-Faktor-Authentifizierung (2FA).

(2) Kennwörter müssen mindestens 12 Zeichen umfassen und sind alle 90 Tage zu wechseln.

### § 4.3 E-Mail-Signatur
(1) Alle ausgehenden E-Mails müssen eine standardisierte Signatur mit folgenden Angaben enthalten:
* Name, Dienststelle, Telefonnummer,
* Rechtlicher Hinweis (z. B. *"Vertraulich – nur für den Adressaten"*),
* Link zur Datenschutzerklärung.

### § 4.4 Protokollierung und Archivierung
(1) E-Mails der Stufen V3 / C–D und V4 / E werden zehn Jahre archiviert.

(2) Zugriffe werden nach § 64 NDSG protokolliert.

### § 4.5 Massenmails
(1) Newsletter und Rundmails an externe Empfängerinnen und Empfänger bedürfen der Genehmigung durch die Pressestelle.

---

## § 5 Umgang mit sensiblen Daten
### § 5.1 Verbotene Inhalte
(1) Folgende Daten dürfen nicht per E-Mail versendet werden:
* Passwörter, Zugangsdaten, Bankverbindungen,
* Daten der Stufen **V4 / E** (z. B. Jugendamtsakten).

### § 5.2 Anlagen
(1) Anhänge sind mit einem Kennwort zu schützen; das Kennwort ist auf einem getrennten Weg zu übermitteln.

(2) Die zulässige Dateigröße beträgt 20 MB. Größere Dateien sind über gesicherte Transfersysteme zu übermitteln.

### § 5.3 Empfangsbestätigungen
(1) Bei E-Mails der Stufen V3 / C–D aufwärts ist eine Lesebestätigung anzufordern.

---

## § 6 Verhalten bei Sicherheitsvorfällen
### § 6.1 Datenpanne
(1) Wer eine Datenpanne bemerkt, meldet sie unverzüglich der oder dem Datenschutzbeauftragten und der IT-Sicherheit.

(2) Die E-Mail ist zurückzurufen, soweit dies technisch möglich ist.

(3) Der Vorgang ist nach Art. 33 DSGVO zu dokumentieren.

### § 6.2 Phishing und Schadsoftware
(1) Anhänge und Verweise aus unbekannten Quellen dürfen nicht geöffnet werden.

(2) Verdächtige E-Mails sind an **it-sicherheit@[kommune].de** weiterzuleiten.

---

## § 7 Schulung und Verantwortlichkeiten
### § 7.1 Schulungen
(1) Alle Beschäftigten werden jährlich geschult.

(2) Neu eintretende Beschäftigte werden vor Aufnahme der Tätigkeit eingewiesen.

### § 7.2 Verantwortlichkeiten
(1) Die IT-Abteilung stellt sichere Systeme bereit und verwaltet die Zertifikate.

(2) Die Fachbereiche stufen E-Mails nach `reg-klassifizierung` ein.

(3) Die oder der Datenschutzbeauftragte überwacht die Einhaltung dieser Dienstanweisung.

---

## § 8 Inkrafttreten und Überprüfung
(1) Diese Dienstanweisung tritt am [Datum] in Kraft.

(2) Sie wird jährlich durch die IT-Sicherheit überprüft.

**Unterschrift:**
[Name], [Position]
[Name der Kommune], [Datum]

---

## Anlagen
1. Richtlinie zur Datenklassifizierung (`reg-klassifizierung`), Anlage B — Umgangsmatrix
2. Muster-E-Mail-Signatur
3. Liste sicherer Behördenpostfächer (EGVP, OSCI)
4. Verfahrensanweisung bei Datenpannen