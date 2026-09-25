---
id: reg-da-loeschung
name: Dienstanweisung Löschung und Löschkonzept (DA Löschung)
typ: Dienstanweisung
status: aktiv
datum: 2026-09-24
zustaendigeEinheit: oe-amt-1-4
entscheidendesGremium: Hauptverwaltungsbeamter
ersetzt: null
---

# Dienstanweisung Löschung und Löschkonzept (DA Löschung)

**Erlassen von der Behördenleitung der Musterkommune am:** [DATUM]
**Inkrafttreten:** [DATUM]
**Verantwortlich für Fortschreibung:** Datenschutzbeauftragte/r (1.4)

---

## § 1 Zweck und Rechtsgrundlagen

(1) Diese Dienstanweisung regelt die Löschung personenbezogener Daten in der Musterkommune. Sie setzt die gesetzlichen Pflichten aus der DSGVO, dem NDSG und dem NArchG in verbindliche Verwaltungsabläufe um.

(2) Rechtsgrundlagen:

- Art. 5 Abs. 1 lit. e) DSGVO — Speicherbegrenzung
- Art. 5 Abs. 2 DSGVO — Rechenschaftspflicht (Löschkonzept)
- Art. 17 DSGVO — Recht auf Löschung
- Art. 19 DSGVO — Mitteilungspflicht an Empfänger
- Art. 25 Abs. 2 DSGVO — Privacy by Default
- § 3 NArchG — Anbietungspflicht an das Niedersächsische Landesarchiv
- § 94 NBG — Löschfristen Personalakten

(3) Maßgebliche Auslegungshilfen:

- LfD Niedersachsen: Hilfestellungen für Verantwortliche bei der
  Festlegung von Löschfristen (2018, Stand 07.09.2018)
- DSK Kurzpapier Nr. 11 — Recht auf Löschung
- BayLfD: Orientierungshilfe „Das Recht auf Löschung" (30.09.2021)
- BayLfD/GDA: Arbeitspapier „Löschung oder Archivierung?" (01.12.2022)
- BSI CON.6 — Löschen und Vernichten (IT-Grundschutz)
- DIN 66399 — Datenträgervernichtung (Sicherheitsstufen 1–5)

## § 2 Begriffsbestimmungen

(1) **Löschung** ist das dauerhafte und unwiederbringliche Entfernen personenbezogener Daten. Eine Sperrung (Einschränkung der Verarbeitung nach Art. 18 DSGVO) ist keine Löschung.

(2) **Einzelfall-Löschung** ist die Löschung einzelner personenbezogener Daten innerhalb laufender Vorgänge (z. B. auf Antrag nach Art. 17 DSGVO, Schwärzung einzelner Einträge).

(3) **Systemimmanente Löschroutine** ist die regelmäßige, vollständige Löschung ganzer Datenbestände nach Ablauf der festgelegten Aufbewahrungsfristen (z. B. Aussonderung eines kompletten Aktenjahrgangs).

(4) **Löschungssurrogat** ist die Übernahme von Unterlagen durch das zuständige Archiv. Die Übernahme tritt für die abgebende Stelle an die Stelle der Löschung. Die Löschungspflicht entfällt.

## § 3 Löschkonzept

(1) Jede Organisationseinheit führt ein Löschkonzept. Das Löschkonzept enthält für jede Datenkategorie:

- die festgelegte Löschfrist (Art. 30 Abs. 1 lit. f DSGVO)
- die Rechtsgrundlage der Frist
- die verantwortliche Person
- den Prüfrhythmus (jährlich)
- den Löschzeitpunkt (Fristbeginn)
- die technische Löschmethode (TOM)

(2) Bei der Festlegung von Löschfristen ist die **Hilfestellung der LfD Niedersachsen zu Löschfristen** (2018) heranzuziehen. Die dort genannten Regelungen (insb. Nr. 9.2 d Nds. AktO, §§ 94 ff. NBG, § 28 NDSG) sind als Orientierung heranzuziehen.

## § 4 Löschfristen (Niedersachsen)

Die folgende Tabelle gilt als Orientierungsrahmen für die Fristenfestlegung. Abweichungen durch Spezialgesetze gehen vor.

| Datenkategorie | Löschfrist | Rechtsgrundlage |
|---------------|-----------|-----------------|
| PbD im Anwendungsbereich DSGVO | unverzüglich (2–4 Wochen, Einzelfallprüfung) | Art. 17 DSGVO, Nr. 9.2 d Nds. AktO |
| PbD — JI-RL (NDSG Teil 2) | 15 Jahre (verkürzbar auf 5) | § 28 NDSG |
| Bewerbungsunterlagen | 5 Monate – 1 Jahr | § 88 Abs. 1 NBG, § 15 Abs. 4 AGG |
| Personalakten | 5 Jahre nach Abschluss | § 94 Abs. 1, 4 NBG |
| Erkrankungen, Beihilfen, Heilfürsorge | 5 Jahre nach Abschluss | § 94 Abs. 2 S. 1 NBG |
| Erholungsurlaub | 3 Jahre nach Abschluss | § 94 Abs. 2 S. 1 NBG |
| Versorgungsakten | 5 Jahre (Wiederaufleben: 30) | § 94 Abs. 3, 4 NBG |
| Zeiterfassungsdaten | 6 Monate / unverzüglich | Erforderlichkeitsprinzip, TVöD § 37 |
| Telekommunikations-Verkehrsdaten | unverzüglich nach Verbindung | § 96 TKG |
| Entgeltabrechnung TK | spätestens 6 Monate | § 97 Abs. 3 TKG |
| Sonstige fachspezifische Fristen | siehe Anlage 1 | vgl. LfD Nds (2018), S. 3 |

(2) **Fristbeginn:** Die Löschfrist beginnt mit dem Ende des Jahres, in dem der Vorgang abgeschlossen wurde, sofern keine speziellere Regelung greift.

## § 5 Einzelfall-Löschung vs. Systemroutine

(1) **Einzelfall-Löschung** — Vorgehen nach Antrag (Art. 17 DSGVO):

- Der DSB prüft den Antrag nach dem Prozess `proc-loeschung-antrag`.
- Einzelfall-Löschungen sind auch innerhalb laufender Vorgänge und
  vor Ablauf der Aufbewahrungsfrist zulässig, wenn ein Löschungsgrund
  nach Art. 17 Abs. 1 DSGVO vorliegt und kein Ausnahmetatbestand
  nach Art. 17 Abs. 3 DSGVO greift.
- Eine archivrechtliche Anbietung ist nicht erforderlich.
- Ggf. reicht eine Schwärzung einzelner Einträge.

(2) **Systemimmanente Löschroutine** — periodische Aussonderung:

- Vor der Löschung ganzer Datenbestände ist **zwingend** das
  zuständige Archiv anzubieten (§ 3 NArchG).
- Die Anbietung erfolgt 30 Jahre nach Entstehung der Unterlagen,
  sofern keine andere Anbietungsfrist gilt.
- Übernimmt das Archiv die Unterlagen → Löschungssurrogat
  (Löschungspflicht entfällt).
- Lehnt das Archiv die Übernahme ab → zwingende Löschung.
- Eine Löschung ohne vorherige Anbietung ist unzulässig.

## § 6 Technisch-organisatorische Maßnahmen (TOM)

(1) Die technische Löschung muss die betroffenen Daten dauerhaft und unwiederbringlich entfernen. Maßstab für digitale Datenträger: BSI CON.6 (Löschen und Vernichten). Maßstab für physische Datenträger: DIN 66399 (Sicherheitsstufen 1–5).

(2) Die konkrete Löschmethode richtet sich nach:

- der Schutzstufe der Daten (A–E nach LfD-Konzept)
- dem Datenträgertyp (Papier, Festplatte, SSD, optische Medien)
- der technischen Löschbarkeit (bei SSDs: Secure Erase, keine
  herkömmlichen Überschreibverfahren)

(3) Die IT-Abteilung stellt sicher, dass Löschfunktionen in allen IT-Verfahren vorhanden und dokumentiert sind. Bereits bei der Einführung neuer Verfahren ist die technische Löschbarkeit zu prüfen (Privacy by Default, Art. 25 Abs. 2 DSGVO).

(4) Löschvorgänge sind zu protokollieren (Löschprotokoll: was, wann, wie, durch wen).

## § 7 Archivierung

(1) Vor jeder systemimmanenten Löschroutine ist das zuständige Archiv anzubieten (§ 3 NArchG). Die Anbietungspflicht gilt für alle Unterlagen, die zur Aufgabenerfüllung nicht mehr benötigt werden.

(2) Übernimmt das Archiv die Unterlagen, tritt die Übernahme an die Stelle der Löschung (Löschungssurrogat). Die Löschungspflicht der abgebenden Stelle entfällt.

(3) Bei Einzelfall-Löschungen, die nicht anlasslos ganze Bestände betreffen (Art. 17-Antrag, Korrektur unrichtiger Daten), ist eine Anbietung nicht erforderlich. Die berechtigte Löschung einzelner Daten im laufenden Verwaltungsbetrieb wird durch die archivrechtliche Anbietungspflicht nicht blockiert, solange die Anbietungspflicht noch nicht eingetreten ist.

(4) Die abgebende Stelle hat keine Informationspflicht nach Art. 13 oder 14 DSGVO gegenüber dem Archiv. Die Übergabe ist nicht als Zweckänderung anzusehen (Art. 5 Abs. 1 lit. b DSGVO).

## § 8 Verantwortlichkeiten

| Rolle | Aufgabe | RASCI |
|-------|---------|-------|
| Fachverantwortliche | Löschkonzept führen, Löschung durchführen, Fristen überwachen | R |
| Datenschutzbeauftragte/r | Löschkonzept prüfen/freigeben, Anträge koordinieren, Art. 19-Mitteilungen veranlassen | A |
| Rechtsabteilung | Ausnahmetatbestände prüfen | C |
| IT-Abteilung | Technische Löschbarkeit sicherstellen, Löschprotokolle | S |
| Archiv | Archivwürdigkeit prüfen, Übernahme/Löschungssurrogat | C |

## § 9 Dokumentation und Nachweispflicht

(1) Jede Löschung ist zu dokumentieren (Rechenschaftspflicht Art. 5 Abs. 2 DSGVO):

- bei Einzelfall-Löschungen: in der Verwaltungsakte
- bei systemimmanenten Routinen: im Löschprotokoll

(2) Dokumentationsumfang: was wurde gelöscht, wann, durch wen, aufgrund welcher Rechtsgrundlage, ggf. Art. 19-Mitteilungen.

(3) Die Löschdokumentation unterliegt ihrerseits den Fristen des Löschkonzepts.

## § 10 Schulung und Sensibilisierung

(1) Alle Beschäftigten werden jährlich über die Löschfristen und den Prozess zur Bearbeitung von Löschungsanträgen geschult.

(2) Die IT-Abteilung schult die Anwender in den Löschfunktionen der eingesetzten Fachverfahren.

## § 11 Inkrafttreten

Diese Dienstanweisung tritt am [DATUM] in Kraft.

[ORT], den [DATUM]

________________________________
[UNTERSCHRIFT BÜRGERMEISTER/IN]
