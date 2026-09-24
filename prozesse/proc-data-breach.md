---
id: proc-data-breach
titel: Datenschutzverletzung melden und bearbeiten (Data Breach)
status: aktiv
zustaendigeEinheit: oe-amt-10
zustaendigeRolle: datenschutzbeauftragte
beteiligte:
- rolle: datenschutzbeauftragte
  phase: 1,2,3,4,5
  aufgabe: Bewertung, Meldung an Aufsichtsbehörde, Betroffenenbenachrichtigung, Dokumentation
- rolle: it-abteilung
  phase: '1'
  aufgabe: Technische Sofortmaßnahmen, Ursachenanalyse, forensische Sicherung
- rolle: fachverantwortliche
  phase: '1,5'
  aufgabe: Unverzügliche Meldung an DSB, Umsetzung von Verbesserungsmaßnahmen
- rolle: rechtsabteilung
  phase: '2'
  aufgabe: Rechtliche Bewertung, Prüfung Strafanzeige
- rolle: oeffentlichkeitsarbeit
  phase: '3'
  aufgabe: Externe Kommunikation, Pressemitteilung
beteiligte_extern:
- rolle: aufsichtsbehoerde
  phase: '3'
  aufgabe: Entgegennahme und Prüfung der Meldung
daten:
  input: []
  output: []
  datenspeicher:
  - id: dstore-sicherheitsmangelmeldung
  - id: dstore-hinweismeldung
  - id: dstore-verwaltungsakte
regelungen:
- Art. 33 DSGVO – Meldung von Datenschutzverletzungen an die Aufsichtsbehörde (72h-Frist)
- Art. 34 DSGVO – Benachrichtigung der betroffenen Personen bei hohem Risiko
- Art. 5 Abs. 2 DSGVO – Rechenschaftspflicht und Dokumentation
- Art. 32 DSGVO – Sicherheit der Verarbeitung (TOM)
- Art. 4 Nr. 12 DSGVO – Definition „Datenschutzverletzung"
- EDPB-Leitlinien 9/2022 (v2.0, März 2023) – Auslegungshilfe zu Art. 33/34 DSGVO
leika_id: ''
ozg_id: ''
letzte-aktualisierung: '2026-09-23'
---

# Datenschutzverletzung melden und bearbeiten

**An wen wende ich mich?** Jeder Beschäftigte, der Kenntnis von einer
möglichen Datenschutzverletzung erlangt, meldet diese unverzüglich dem
Datenschutzbeauftragten (Amt 10). Der DSB übernimmt die weitere
Bearbeitung, Bewertung und ggf. die Meldung an die LfD Niedersachsen.

**Verwandte Wissensseite:** `wiki/O/Prozess-Data-Breach.md`

## Prozessschritte

**01 Datenschutzverletzung erkennen und melden**
*Jeder Beschäftigte meldet einen Verdacht unverzüglich an den DSB.
IT-Abteilung leitet sofort technische Sofortmaßnahmen ein (betroffene
Systeme vom Netz trennen, Zugriffe sperren, Logs sichern). Die
Fachverantwortlichen stellen sicher, dass keine Meldung verloren geht.
Der DSB dokumentiert den Eingang mit Datum und Uhrzeit — dieser
Zeitpunkt bestimmt den Fristbeginn (72h).*

**02 Erstbewertung: Liegt eine Datenschutzverletzung vor?**
*DSB prüft anhand der Zwei-Elemente-Prüfung (EDPB 9/2022):
1. Verletzungsverhalten (Sicherheitsverletzung: Verstoß gegen Dienstanweisung,
   Überwindung technischer Vorkehrungen, organisatorisches Fehlverhalten)
2. Verletzungserfolg (Vertraulichkeit, Integrität oder Verfügbarkeit
   beeinträchtigt?). Bei unklarer Lage: vom Schlimmsten ausgehen.
   Rechtsabteilung prüft, ob Strafanzeige sinnvoll ist (BayLfD AKI 57).*

**03 Risikobewertung und Meldepflicht prüfen**
*DSB bewertet das Risiko anhand: Art und Sensitivität der Daten,
Identifizierbarkeit der Betroffenen, Schwere möglicher Folgen
(Identitätsdiebstahl, Diskriminierung, finanzielle Verluste), Anzahl
der Betroffenen, besondere Kategorien nach Art. 9 DSGVO.
Drei Stufen:
- Kein Risiko → dokumentieren, keine Meldung
- Risiko → Meldung an LfD nach Art. 33 DSGVO
- Hohes Risiko → Meldung + Betroffenenbenachrichtigung nach Art. 34*

**04 Meldung an die Aufsichtsbehörde (innerhalb 72h)**
*DSB meldet binnen 72 Stunden nach Bekanntwerden an die LfD
Niedersachsen. Inhalt: Art der Verletzung, Datenkategorien, ungefähre
Zahl der Betroffenen/Datensätze, wahrscheinliche Folgen, ergriffene
oder vorgeschlagene Maßnahmen, DSB-Kontaktdaten. Falls noch nicht alle
Informationen vorliegen: schrittweise Meldung — Erstmeldung jetzt,
Folgemeldungen sobald verfügbar.*

**05 Betroffene benachrichtigen (bei hohem Risiko)**
*DSB benachrichtigt die betroffenen Personen unverzüglich in klarer,
einfacher Sprache: Art der Verletzung, wahrscheinliche Folgen,
ergriffene und empfohlene Maßnahmen zur Schadensminderung,
DSB-Kontaktdaten. Öffentlichkeitsarbeit unterstützt bei
Pressemitteilungen, falls die Verletzung öffentlich bekannt wird.
Keine Benachrichtigung bei wirksamer Verschlüsselung oder wenn
nachfolgende Maßnahmen das hohe Risiko beseitigen.*

**06 Nachbearbeitung und Abschluss**
*DSB dokumentiert den gesamten Vorfall (Art. 33 Abs. 5 DSGVO): Fakten,
Folgen, ergriffene Maßnahmen, Kommunikation mit Aufsichtsbehörde und
Betroffenen. IT-Abteilung analysiert Ursachen und passt TOM an.
Fachverantwortliche setzen Prozessverbesserungen um. Ggf. Schulungen
der Beschäftigten. Abschlussbericht an LfD nach Aufklärung.*

---

*Dieser Entwurf wurde mit KI-Unterstützung erstellt. Inhaltliche Prüfung durch den Menschen erforderlich.*