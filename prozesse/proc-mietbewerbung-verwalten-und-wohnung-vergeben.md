---
id: proc-mietbewerbung-verwalten-und-wohnung-vergeben
titel: Mietbewerbung verwalten und Wohnung vergeben
status: aktiv
zustaendigeEinheit: oe-amt-23
zustaendigeRolle: ''
beteiligte:
- einheit: oe-amt-65
  aufgabe: ''
daten:
  input: []
  output: []
  datenspeicher:
  - id: dstore-bewerbungsunterlagen
  - id: dstore-wohnberechtigung
  - id: dstore-einkommensnachweise-haushalt
  - id: dstore-wohnungszuordnungsmerkmal
regelungen:
- Art. 6 Abs. 1 lit. b) DSGVO - vorvertragliche Verarbeitung auf Anfrage der bewerbenden
  Person
- Art. 6 Abs. 1 lit. e) DSGVO, § 3 NDSG - Vergabe kommunalen Wohnraums
- § 19 Abs. 3 AGG - zulässige unterschiedliche Behandlung zur Schaffung und Erhaltung
  sozial stabiler Bewohnerstrukturen
- § 19 Abs. 5 Satz 3 AGG - Schwelle von 50 Wohnungen für die Einordnung als Massengeschäft
- § 21 Abs. 5 AGG - Zweimonatsfrist für Ansprüche wegen Benachteiligung
- § 22 AGG - Beweislast bei Indizien für eine Benachteiligung
- WoFG - Wohnberechtigungsschein bei gefördertem Wohnraum
- Art. 9 Abs. 2 lit. a) DSGVO - freiwillige Angaben zu Behinderung oder gesundheitlicher
  Dringlichkeit
- §§ 535 ff. BGB - Mietvertrag im Anschluss
leika_id: null
ozg_id: null
letzte-aktualisierung: '2026-07-30'
---

# Mietbewerbung verwalten und Wohnung vergeben

## Zweck

Entgegennahme und Verwaltung von Bewerbungen um kommunale Mietwohnungen, Auswahl der Mieterin oder des Mieters und Dokumentation der Auswahlentscheidung.

## Prozessschritte

**01 Bewerbung aufnehmen**
*Erhoben werden Name, Anschrift und Kontaktdaten, Haushaltsgröße und -zusammensetzung, die bisherige Wohnsituation und der Wohnungswunsch. Bei gefördertem Wohnraum wird der Wohnberechtigungsschein verlangt; ohne ihn besteht kein Zugang zu diesem Bestand.*

**02 Freiwillige Angaben getrennt behandeln**
*Angaben zu einer Behinderung, zu Barrierefreiheitsbedarf oder zu einer gesundheitlichen Dringlichkeit sind **freiwillig**. Niemand muss sie machen, um sich zu bewerben; wer sie macht, tut es zum eigenen Vorteil. Grundlage ist deshalb Art. 9 Abs. 2 lit. a) DSGVO. Die Angabe wird gesondert geführt, der Einwilligungs- und Widerrufsstand vermerkt; ein Widerruf führt zur Löschung der Angabe, nicht der Bewerbung.*

**03 Einkommen nur prüfen, soweit erforderlich**
*Einkommensangaben werden erhoben, soweit sie für den Wohnberechtigungsschein, für die Prüfung der Mietzahlungsfähigkeit oder für ein Vergabekriterium nach § 19 Abs. 3 AGG gebraucht werden. Belege werden nach der Prüfung nicht dauerhaft vorgehalten; festgehalten wird das Prüfergebnis.*

**04 Auswahlkriterien anwenden und dokumentieren**
*Die Auswahl richtet sich nach den festgelegten Vergabekriterien. § 19 Abs. 3 AGG erlaubt eine unterschiedliche Behandlung im Hinblick auf sozial stabile Bewohner- und ausgewogene Siedlungsstrukturen -- dies ist zugleich die Rechtfertigung dafür, die zugrunde liegenden Haushaltsdaten überhaupt zu erheben. **Die Entscheidung wird mit Begründung festgehalten**; nach § 22 AGG trägt die Kommune die Beweislast, sobald Indizien für eine Benachteiligung vorliegen.*

**05 Wohnung anbieten**
*Das Angebot ergeht an die ausgewählte Person; die für den Vertragsschluss zuständige Stelle erhält nur die dafür erforderlichen Daten, nicht die gesamte Bewerbungsakte.*

**06 Absagen und Frist wahren**
*Nicht berücksichtigte Bewerbungen werden abgesagt. Bewerbung und Auswahlentscheidung werden sechs Monate aufbewahrt -- die Zweimonatsfrist des § 21 Abs. 5 AGG zuzüglich eines Zuschlags für Zustellung und Klageerhebung.*

**07 Übergang in die Mietakte**
*Bei erfolgreicher Bewerbung gehen die für das Mietverhältnis erforderlichen Daten in die Mietakte über; der Vertragsschluss wird in `proc-mietvertrag-fuer-staedtische-wohnung` geführt. Die übrigen Bewerbungsunterlagen werden nach Abschluss des Vergabeverfahrens gelöscht.*

**08 Löschen**
*Abgelehnte Bewerbungen einschließlich der Auswahldokumentation werden sechs Monate nach der Absage gelöscht -- Festlegung des Trägers. Freiwillige Angaben nach Art. 9 DSGVO werden bei Widerruf unverzüglich gelöscht.*

**Herkunft des Schrittblocks:** abgeleitet aus §§ 19, 21 und 22 AGG, dem WoFG und §§ 535 ff. BGB, nicht aus einer Ablauferhebung im Amt 23.
