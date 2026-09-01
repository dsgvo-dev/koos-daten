---
id: reg-isl
name: Informationssicherheitsleitlinie (ISL)
typ: Leitlinie
zustaendigeEinheit: oe-amt-1-5
datum: "2026-06-07"
status: entwurf
version: 1.0
basierend_auf:
  - BSI-Standard 200-1 (ISMS)
  - BSI-Standard 200-2 (IT-Grundschutz-Methodik)
  - BSI-Standard 200-3 (Risikomanagement)
  - ISB-Rolle (dsms:dsms/Organisation/Rolle-ISB.md, O.1.R.4)
  - Rolle-Hauptverantwortliche (dsms:dsms/Organisation/Rolle-Hauptverantwortliche.md, O.1.R.1)
rechtsgrundlagen:
  - BSI IT-Grundschutz (Standards 200-1 bis 200-4)
  - [Landesrechtliche IT-Sicherheitsregelungen]
  - DSGVO Art. 32 (Technisch-organisatorische Maßnahmen)
  - [Landesdatenschutzgesetz]
---

# Informationssicherheitsleitlinie (ISL)

## für die [Stadt/Gemeinde/Landkreis] [NAME]

**Erlassen von der Behördenleitung am:** [DATUM]
**Inkrafttreten:** [DATUM]
**Verantwortlich für Fortschreibung:** Informationssicherheitsbeauftragte/r (ISB)
**Evaluierung:** jährlich, erstmals zum [DATUM + 1 Jahr]

---

## 1. Präambel und Zweck

(1) Die [Stadt/Gemeinde/Landkreis] [NAME] ist als Teil der öffentlichen Verwaltung auf eine sichere, verfügbare und vertrauliche Verarbeitung von Informationen angewiesen. Der Schutz von Informationen — gleich ob digital oder analog — ist Voraussetzung für die Aufgabenerfüllung, das Vertrauen der Bürgerinnen und Bürger sowie die Rechtskonformität des Verwaltungshandelns.

(2) Diese Leitlinie definiert die **grundlegenden Ziele, Prinzipien und die Organisation** der Informationssicherheit in der Verwaltung. Sie ist das zentrale Strategiedokument des **Informationssicherheits-Managementsystems (ISMS)** und richtet sich an alle Beschäftigten.

(3) Die Leitlinie folgt den **BSI-Standards 200-1 (ISMS), 200-2 (IT-Grundschutz-Methodik) und 200-3 (Risikomanagement)**. Sie ist kompatibel zur ISO/IEC 27001 und wird im Rahmen des PDCA-Prozesses (Plan-Do-Check-Act) kontinuierlich fortgeschrieben.

(4) Die Behördenleitung bekennt sich zu dieser Leitlinie und stellt die erforderlichen Ressourcen bereit (personell, technisch, finanziell).

---

## 2. Geltungsbereich

(1) **Sachlich:** Diese Leitlinie gilt für alle Informationen, Informationssysteme, IT-Verfahren und Datenverarbeitungen der Verwaltung — unabhängig davon, ob sie digital, analog oder in hybriden Prozessen verarbeitet werden.

(2) **Persönlich:** Sie gilt für alle Beschäftigten der [Stadt/Gemeinde/Landkreis] [NAME], einschließlich Beamtinnen und Beamte, Tarifbeschäftigte, Auszubildende, Praktikantinnen und Praktikanten, Ehrenamtliche sowie externe Dienstleister im Rahmen ihrer Tätigkeit für die Verwaltung.

(3) **Räumlich:** Sie gilt an allen Dienstorten sowie bei mobiler Arbeit, Home-Office, Dienstreisen und Außenterminen.

(4) **Ausgenommen:** Vom Geltungsbereich ausgenommen sind Informationen, die gesonderten Geheimschutzregelungen unterliegen (soweit nicht durch spezifische Sicherheitsvereinbarungen abgedeckt).

---

## 3. Ziele der Informationssicherheit

### 3.1 Schutzziele nach BSI

Die Informationssicherheit verfolgt folgende **Schutzziele**, die für alle Informationen und IT-Verfahren gleichermaßen gelten:

| Schutzziel | Definition |
|------------|------------|
| **Vertraulichkeit** | Informationen sind nur Befugten zugänglich (Need-to-Know-Prinzip) |
| **Integrität** | Informationen sind vollständig, richtig und nicht unbefugt verändert |
| **Verfügbarkeit** | Informationen und Systeme stehen im erforderlichen Umfang und Zeitrahmen zur Verfügung |

### 3.2 Erweiterte Schutzziele

Ergänzend gelten für bestimmte Verfahren:

| Erweitertes Schutzziel | Definition |
|------------------------|------------|
| **Authentizität** | Die Identität von Kommunikationspartnern und Systemen ist nachweisbar |
| **Nichtabstreitbarkeit** | Durchgeführte Aktionen sind nachweisbar und können nicht abgestritten werden |
| **Belastbarkeit** | Systeme widerstehen Störungen und erholen sich zuverlässig (Resilienz) |

### 3.3 Übergeordnete Ziele

- Sicherstellung des **rechtskonformen** Betriebs aller IT-Verfahren.
- Schutz der **Bürgerdaten** vor Verlust, Missbrauch und unbefugtem Zugriff.
- Sicherung der **Handlungsfähigkeit** der Verwaltung auch bei IT-Störungen oder -Ausfällen.
- **Risikogerechte** Absicherung — der Aufwand der Schutzmaßnahmen steht im Verhältnis zum Schutzbedarf.

---

## 4. Organisation der Informationssicherheit

### 4.1 Verantwortlichkeiten

#### Behördenleitung (Hauptverantwortliche, O.1.R.1)

(1) Die Behördenleitung trägt die **Gesamtverantwortung** für die Informationssicherheit. Sie erlässt diese Leitlinie und stellt die Ressourcen für das ISMS bereit.

(2) Sie ernennt eine Informationssicherheitsbeauftragte oder einen Informationssicherheitsbeauftragten (ISB) und stattet diese Person mit den erforderlichen Befugnissen und Ressourcen aus.

(3) Sie entscheidet über grundsätzliche Sicherheitsfragen, über die Annahme von Restrisiken und über das Sicherheitsbudget.

#### Informationssicherheitsbeauftragte/r (ISB, O.1.R.4)

(1) Der ISB ist für den **Aufbau, Betrieb und die Fortschreibung des ISMS** verantwortlich. Er berichtet direkt an die Behördenleitung.

(2) Aufgaben:
- Erstellung und Fortschreibung dieser Leitlinie und aller untergeordneten Sicherheitsrichtlinien.
- Durchführung von Schutzbedarfsfeststellungen und Risikoanalysen.
- Beratung der Fachbereiche und der IT-Abteilung in Sicherheitsfragen.
- Koordination von Sicherheitsvorfällen und Notfallmanagement.
- Planung und Durchführung von Sicherheitsschulungen.
- Regelmäßige Berichterstattung an die Behördenleitung.

(3) Der ISB ist fachlich weisungsfrei und hat ein uneingeschränktes Auskunfts- und Akteneinsichtsrecht in allen Sicherheitsfragen.

#### Führungskräfte (Fachverantwortliche, O.1.R.2)

(1) Führungskräfte sind für die Einhaltung der Sicherheitsvorgaben in ihrem Verantwortungsbereich verantwortlich.

(2) Sie sorgen für die Sensibilisierung und Schulung ihrer Mitarbeitenden und melden Sicherheitsvorfälle unverzüglich an den ISB.

(3) Sie wirken bei Schutzbedarfsfeststellungen und Risikoanalysen für ihre Verfahren mit.

#### IT-Abteilung (O.1.R.3)

(1) Die IT-Abteilung setzt die vom ISB vorgegebenen Sicherheitsmaßnahmen technisch um.

(2) Sie betreibt die Systeme sicherheitskonform, dokumentiert Konfigurationen und meldet Sicherheitsvorfälle an den ISB.

(3) Sie unterstützt den ISB bei der technischen Analyse von Sicherheitsvorfällen.

#### Alle Beschäftigten

(1) Alle Beschäftigten sind verpflichtet, die Sicherheitsvorgaben einzuhalten, mit Informationen sorgsam umzugehen und Sicherheitsvorfälle oder -schwachstellen unverzüglich zu melden.

(2) Sie nehmen an den verpflichtenden Sicherheitsschulungen teil.

### 4.2 Gremien

| Gremium | Mitglieder | Aufgaben | Turnus |
|---------|-----------|----------|--------|
| **Sicherheitsforum** (Steuerkreis ISMS) | Behördenleitung, ISB, IT-Leitung, DSB, Organisation | Strategische Steuerung, Ressourcenentscheidung, Annahme von Restrisiken | **halbjährlich** |
| **ISB-IS-Koordination** | ISB, IT-Leitung, DSB, Datenschutzkoordinatoren | Operative Steuerung, Abstimmung konkreter Maßnahmen | **monatlich** |
| **Sicherheitsaudit** | ISB, ggf. externe Prüfer | Überprüfung der Wirksamkeit des ISMS | **jährlich** |

### 4.3 Dokumentation des ISMS

(1) Das ISMS wird in folgenden Dokumenten abgebildet:

| Dokument | Inhalt | Federführung | Fortschreibung |
|----------|--------|-------------|----------------|
| **Informationssicherheits-Leitlinie** (dieses Dokument) | Strategie, Ziele, Organisation | ISB | jährlich |
| **Sicherheitsrichtlinien** | Konkrete Sicherheitsvorgaben (Passwörter, Zugriff, Verschlüsselung, Mobile Geräte, Cloud) | ISB | bei Bedarf, mind. alle 2 Jahre |
| **Schutzbedarfsfeststellung** | Einstufung aller Verfahren in normal/hoch/sehr hoch | ISB + Fachverantwortliche | bei Änderungen, mind. alle 3 Jahre |
| **Risikoanalyse** | Identifikation und Bewertung von Risiken (BSI 200-3) | ISB | bei erhöhtem Schutzbedarf |
| **Notfallhandbuch** | Maßnahmen bei Ausfällen und Störungen | ISB + IT | jährlich |
| **Sicherheitsvorfalls-Register** | Dokumentation aller Sicherheitsvorfälle | ISB | fortlaufend |
| **TOM-Dokumentation** | Technisch-organisatorische Maßnahmen | ISB + IT + DSB | bei Systemänderungen |

(2) Die Dokumente sind revisionssicher zu führen und für die Prüfung durch interne Revision und Aufsichtsbehörden bereitzuhalten.

---

## 5. Grundsätze der Informationssicherheit

### 5.1 Risikoorientierung

(1) Alle Sicherheitsmaßnahmen orientieren sich am **Schutzbedarf** der Informationen und Verfahren. Die Schutzbedarfsfeststellung (normal/hoch/sehr hoch) nach BSI-Standard 200-2 ist der Ausgangspunkt jeder Sicherheitsentscheidung.

(2) Ist der Schutzbedarf **normal**, genügen die Standardmaßnahmen des BSI IT-Grundschutz-Kompendiums (Basis- und Kern-Absicherung).

(3) Ist der Schutzbedarf **hoch** oder **sehr hoch**, ist zusätzlich eine **Risikoanalyse** nach BSI-Standard 200-3 durchzuführen.

### 5.2 PDCA-Prozess

Das ISMS folgt dem **PDCA-Zyklus** (Plan-Do-Check-Act):

```
Plan:   Festlegung von Zielen, Verfahren und Maßnahmen
        ↓
Do:     Umsetzung der Maßnahmen im laufenden Betrieb
        ↓
Check:  Überwachung, Messung, Audit, Überprüfung
        ↓
Act:    Korrektur- und Verbesserungsmaßnahmen
        ↓ (zurück zu Plan)
```

### 5.3 Sicherheit als Gemeinschaftsaufgabe

(1) Informationssicherheit ist keine Aufgabe allein der IT-Abteilung oder des ISB. Sie betrifft alle Ebenen und Funktionen der Verwaltung.

(2) Die IT-Abteilung setzt technische Maßnahmen um. Die Fachbereiche leben die Sicherheitskultur im Arbeitsalltag. Die Führungskräfte tragen Sorge für die Umsetzung in ihren Bereichen.

(3) Der ISB koordiniert, kontrolliert und berät — er entbindet niemanden von seiner eigenen Verantwortung.

### 5.4 Prävention, Detektion, Reaktion

(1) **Prävention:** Sicherheitsmaßnahmen verhindern oder erschweren Sicherheitsvorfälle (Zugriffsschutz, Verschlüsselung, Firewall, Schulung).

(2) **Detektion:** Überwachungs- und Erkennungsmaßnahmen identifizieren Sicherheitsvorfälle frühzeitig (Logging, Monitoring, Alarmierung).

(3) **Reaktion:** Notfallpläne und Wiederherstellungsprozesse stellen die Handlungsfähigkeit auch nach einem Vorfall sicher (Backup, Notfallhandbuch, BCM nach BSI 200-4).

### 5.5 Wirtschaftlichkeit

(1) Der Aufwand für Sicherheitsmaßnahmen muss zum Schutzbedarf und zum erwartbaren Schadensrisiko in angemessenem Verhältnis stehen.

(2) Die Kosten-Nutzen-Abwägung wird vom ISB im Rahmen der Risikoanalyse dokumentiert und im Sicherheitsforum entschieden.

(3) Standardlösungen sind vor Individualentwicklungen zu bevorzugen (Wirtschaftlichkeit, Supportfähigkeit, Prüfbarkeit).

---

## 6. Sicherheitsprozesse

### 6.1 Schutzbedarfsfeststellung und Risikoanalyse

(1) Der ISB führt für jedes IT-Verfahren und jede informationsverarbeitende Einheit eine **Schutzbedarfsfeststellung** hinsichtlich Vertraulichkeit, Integrität und Verfügbarkeit durch. Ergebnis ist eine Einstufung als normal, hoch oder sehr hoch.

(2) Bei Schutzbedarf **hoch** oder **sehr hoch** wird eine **Risikoanalyse** nach BSI-Standard 200-3 durchgeführt.

(3) Die Ergebnisse werden dokumentiert und dem Sicherheitsforum vorgelegt.

### 6.2 Sicherheitsvorfall-Management

(1) Jeder Sicherheitsvorfall (tatsächlich oder vermutet) ist **unverzüglich** dem ISB zu melden.

(2) Der ISB koordiniert die Analyse, Eindämmung und Beseitigung des Vorfalls.

(3) Datenschutzrechtlich relevante Vorfälle sind parallel dem DSB zu melden (Data Breach nach DSGVO Art. 33/34).

(4) Alle Vorfälle werden im **Sicherheitsvorfalls-Register** dokumentiert.

(5) Nach Abschluss erfolgt eine Nachbesprechung und Ableitung von Verbesserungsmaßnahmen.

### 6.3 Änderungsmanagement (Change Management)

(1) Änderungen an IT-Systemen, Verfahren und Sicherheitskonfigurationen sind zu planen, zu dokumentieren und vor der Umsetzung durch den ISB freizugeben.

(2) Wesentliche Änderungen (neue Systeme, Architekturänderungen, Änderungen der Sicherheitsarchitektur) sind dem Sicherheitsforum vorzulegen.

### 6.4 Schulung und Sensibilisierung

(1) Alle Beschäftigten erhalten bei Dienstantritt eine **Grundschulung** zur Informationssicherheit.

(2) Wiederholungsschulungen finden mindestens **alle 2 Jahre** statt.

(3) **Größen-Empfehlung:**
- **S (klein):** Schulung alle 3 Jahre, als Dienstbesprechung oder E-Learning
- **M (mittel):** Schulung alle 2 Jahre, E-Learning mit Präsenz für Risikobereiche
- **L (groß):** Schulung alle 2 Jahre, gestaffelt nach Risikostufen

(4) Beschäftigte in sicherheitskritischen Funktionen (IT-Administration, Berechtigungsverwaltung) erhalten jährliche Spezialschulungen.

### 6.5 Notfallmanagement und BCM

(1) Der ISB erstellt und pflegt ein **Notfallhandbuch** (Business Continuity Management nach BSI-Standard 200-4).

(2) Das Notfallhandbuch enthält:
- Klassifizierung von Notfallszenarien (Ausfall, Datenverlust, Cyberangriff, Naturereignis)
- Eskalationswege und Entscheidungsbefugnisse
- Wiederherstellungspläne (Wiederherstellungszeit RTO, Wiederherstellungspunkt RPO)
- Kommunikationspläne (intern und extern)

(3) Kritische Verfahren werden regelmäßig auf ihre Wiederherstellbarkeit getestet (mindestens **jährlich**).

---

## 7. Umgang mit externen Dienstleistern

(1) Externe Dienstleister, die für die Verwaltung IT-Dienstleistungen erbringen oder Zugriff auf Informationen der Verwaltung haben, sind vertraglich zur Einhaltung der Sicherheitsanforderungen zu verpflichten.

(2) Vor der Beauftragung ist eine **Sicherheitsüberprüfung** durch den ISB durchzuführen.

(3) Bei der Verarbeitung personenbezogener Daten ist ein **Auftragsverarbeitungsvertrag (AVV)** nach Art. 28 DSGVO abzuschließen.

(4) Cloud-Dienste unterliegen einer gesonderten Prüfung (Drittlandsbezug, Datenschutz, Verfügbarkeit, Lock-in-Effekt).

---

## 8. Datenschutz und Informationssicherheit

(1) Informationssicherheit und Datenschutz überschneiden sich bei den **technisch-organisatorischen Maßnahmen** (TOMs nach Art. 32 DSGVO).

(2) Der ISB stimmt alle sicherheitsrelevanten Maßnahmen, die personenbezogene Daten betreffen, mit dem DSB ab.

(3) Bei Zielkonflikten zwischen Sicherheit und Datenschutz entscheidet das Sicherheitsforum unter Beteiligung von ISB und DSB.

(4) Die Datenschutz-Folgenabschätzung (DSFA) nach Art. 35 DSGVO wird vom ISB bei sicherheitsrelevanten Aspekten unterstützt.

---

## 9. Sanktionen und Konsequenzen

(1) Vorsätzliche oder grob fahrlässige Verstöße gegen diese Leitlinie oder die darauf basierenden Sicherheitsrichtlinien können dienst- und arbeitsrechtliche Maßnahmen nach sich ziehen.

(2) Bei Beamtinnen und Beamten gelten die Regelungen des [Landesdisziplinargesetzes]; bei Tarifbeschäftigten die tarif- und arbeitsrechtlichen Regelungen.

(3) Strafrechtlich relevante Sicherheitsverstöße (z. B. Computerbetrug, Datenhehlerei, Ausspähen von Daten) sind der Strafverfolgung zu melden.

---

## 10. Schlussvorschriften

(1) **Aufhebung früherer Regelungen.** Frühere Regelungen zur Informationssicherheit, soweit vorhanden, treten mit Inkrafttreten dieser Leitlinie außer Kraft.

(2) **Verhältnis zu anderen Regelungen.** Die bestehenden Dienstanweisungen (Datenschutz, IT-Nutzung, Korruptionsprävention) bleiben unberührt, soweit sie dieser Leitlinie nicht widersprechen. Sicherheitsspezifische Dienstanweisungen und -richtlinien konkretisieren diese Leitlinie auf der operativen Ebene.

(3) **Veröffentlichung.** Diese Leitlinie wird im Intranet der Verwaltung veröffentlicht und allen Beschäftigten gegen Empfangsbestätigung ausgehändigt.

(4) **Fortschreibung.** Diese Leitlinie wird jährlich durch den ISB überprüft und fortgeschrieben. Änderungen bedürfen der Zustimmung der Behördenleitung.

(5) **Evaluierung.** Die Wirksamkeit dieser Leitlinie und des ISMS wird erstmals **[12 Monate nach Inkrafttreten]** durch ein Sicherheitsaudit überprüft.

(6) **Inkrafttreten.** Diese Leitlinie tritt am [INKRAFTTRETENSDATUM] in Kraft.

---

[ORT], den [DATUM]

__________________________________
[Behördenleitung (Bürgermeister/in / Landrat/Landrätin)]

__________________________________
[Informationssicherheitsbeauftragte/r (ISB)]

---

## Anlage 1 — Begriffsdefinitionen

| Begriff | Definition |
|---------|------------|
| **ISMS** | Informationssicherheits-Managementsystem — Gesamtheit von Richtlinien, Prozessen, Maßnahmen und Verantwortlichkeiten zur Steuerung der Informationssicherheit |
| **ISB** | Informationssicherheitsbeauftragte/r |
| **Schutzbedarf** | Erforderliches Schutzniveau eines Verfahrens hinsichtlich Vertraulichkeit, Integrität und Verfügbarkeit |
| **Risiko** | Kombination aus Eintrittswahrscheinlichkeit eines Schadensereignisses und dessen Schadenshöhe |
| **Restrisiko** | Nach Umsetzung der Sicherheitsmaßnahmen verbleibendes Risiko, das von der Behördenleitung bewusst getragen wird |
| **RTO** | Recovery Time Objective — maximale tolerierbare Ausfallzeit |
| **RPO** | Recovery Point Objective — maximal tolerierbarer Datenverlust |
| **BCM** | Business Continuity Management — Aufrechterhaltung kritischer Geschäftsprozesse bei Störungen |
| **TOM** | Technisch-organisatorische Maßnahmen nach Art. 32 DSGVO |

---

## Anlage 2 — Sicherheitsrichtlinien (Übersicht)

Diese Leitlinie wird durch folgende operative Sicherheitsrichtlinien konkretisiert (jeweils als separates Dokument):

| Richtlinie | Gegenstand | Federführung |
|------------|-----------|-------------|
| Passwort- und Authentifizierungsrichtlinie | Mindestanforderungen an Passwörter, Multi-Faktor-Authentifizierung | ISB + IT |
| Zugriffsberechtigungsrichtlinie | Berechtigungsvergabe, Rezertifizierung, Need-to-Know | ISB + IT |
| Richtlinie Mobile Geräte | Nutzung von Smartphones, Tablets, Laptops außerhalb der Dienststelle | ISB + IT |
| Verschlüsselungsrichtlinie | Anforderungen an Verschlüsselung (Festplatten, Datenträger, Übertragung) | ISB + IT |
| Cloud-Nutzungsrichtlinie | Nutzung von Cloud-Diensten (Drittlandsbezug, AVV, Datenschutz) | ISB + DSB + IT |
| Richtlinie Externe Dienstleister | Sicherheitsanforderungen an Dritte, Vertragsklauseln | ISB + Rechtsabteilung |

---

> **Hinweis:** Diese Leitlinie wurde mit Unterstützung durch KI erstellt und ersetzt keine fachliche Prüfung durch den ISB und die Rechtsabteilung. Vor Erlass ist sie durch die Behördenleitung zu verabschieden.