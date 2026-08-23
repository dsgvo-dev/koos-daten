---
id: proc-eigenschaden-ksa-melden
titel: Eigenschaden melden und an KSA weiterleiten
status: aktiv
zustaendigeEinheit: oe-amt-10
zustaendigeRolle: Sachbearbeitung
beteiligte:
  - einheit: oe-amt-11
    aufgabe: Prüfung des Regresses bei grober Fahrlässigkeit, Mitteilung an die/den Beschäftigten
  - einheit: oe-amt-20
    aufgabe: Zahlungsabwicklung bei Regressforderungen und KSA-Beiträgen
  - einheit: oe-amt-30
    aufgabe: Rechtliche Prüfung bei Streitfällen zur Haftungsquote und zum Regress
daten:
  input:
    - Meldung der/des Beschäftigten oder der Führungskraft (Schadenshergang, Ort, Zeit, Beteiligte)
  output:
    - KSA-Schadensmeldung, Regressbescheid (bei grober Fahrlässigkeit), Abschlussvermerk
  datenspeicher:
    - id: dstore-kfz-daten
    - id: dstore-sicherheitsmangelmeldung
    - id: dstore-zeugenangaben-schadensfall
regelungen:
  - "§ 90 NBG (Schadensersatzpflicht der Beamtin/des Beamten)"
  - "§ 75 BBG (Beamtenhaftung, bundesrechtlicher Hintergrund)"
  - "§§ 280, 619a BGB (Arbeitnehmerhaftung)"
  - "Grundsätze der beschränkten Arbeitnehmerhaftung (BAG, st. Rspr.)"
  - "KSA-Satzung und Verrechnungsgrundsätze für Haftpflichtschäden"
  - "§ 86 NKomVG (Verwaltungsorganisation, Vermögensverwaltung)"
  - "Art. 6 Abs. 1 lit. e DSGVO, § 3 NDSG (Aufgabenerfüllung)"
leika_id: null
ozg_id: null
letzte-aktualisierung: '2026-08-23'
---
# Eigenschaden melden und an KSA weiterleiten

## Zweck

Meldung eines Schadens, den eine oder ein Beschäftigter in Ausübung der dienstlichen Tätigkeit verursacht hat — etwa ein Unfall mit einem Dienstfahrzeug, die Beschädigung von Dienstgeräten oder sonstigem städtischen Eigentum. Die Meldung erfolgt unverzüglich an das Hauptamt (oe-amt-10), das den Schaden aufnimmt, dokumentiert und an den Kommunalen Schadenausgleich (KSA) Hannover weiterleitet. Der KSA reguliert den Schaden als Haftpflichtversicherer der Kommune. Bei grober Fahrlässigkeit ist ein Regress gegen die oder den Beschäftigten zu prüfen; bei einfacher Fahrlässigkeit entfällt dieser nach den Grundsätzen der beschränkten Arbeitnehmerhaftung.

**Anlaufstelle bei Eigenschaden:** Unverzügliche Meldung an die vorgesetzte Führungskraft. Diese leitet den Vorgang an das Hauptamt (oe-amt-10) weiter.

## Prozessschritte

**01 Schaden verursachen und unverzüglich melden**
*Die oder der Beschäftigte meldet den verursachten Schaden unverzüglich ihrer oder seiner vorgesetzten Führungskraft. Die Meldung enthält: Hergang, Ort und Zeitpunkt des Schadens, beteiligte Personen und (bei Dienstfahrzeugen) das Kennzeichen. Bei Unfall mit Personenschaden ist zusätzlich die Polizei zu informieren. Die Führungskraft leitet den Vorgang an das Hauptamt (oe-amt-10) weiter.*

**02 Schaden aufnehmen und dokumentieren**
*Das Hauptamt nimmt den Schaden auf und dokumentiert ihn: Schadensbeschreibung, Fotos, Zeugenangaben, Schadenshöhe (erste Schätzung). Der oder dem Beschäftigten wird Gelegenheit zur Stellungnahme gegeben. Bei Dienstfahrzeugen werden die Kfz-Daten (dstore-kfz-daten) erfasst. Der Vorgang wird in der dstore-sicherheitsmangelmeldung dokumentiert.*

**03 Haftungsquote und Verschuldensgrad prüfen**
*Das Hauptamt prüft den Verschuldensgrad der oder des Beschäftigten: Vorsatz (nie versichert/nie regressfrei), grobe Fahrlässigkeit (Regress möglich), einfache Fahrlässigkeit (kein Regress nach den Grundsätzen der beschränkten Arbeitnehmerhaftung). Bei Zweifeln wird das Rechtsamt (oe-amt-30) beteiligt. Die Prüfung dient der Entscheidung, ob der KSA den Schaden vollständig trägt oder ob ein Regress gegen die oder den Beschäftigten eingeleitet wird.*

**04 KSA-Schadensmeldung einreichen**
*Das Hauptamt erstellt die Schadensmeldung an den KSA Hannover nach dessen Vorgaben (i.d.R. über das KSA-Meldeformular). Die Meldung enthält: Mitgliedsnummer der Kommune, Schadensdatum und -ort, Hergang, Schadenshöhe, Angaben zur/zum Schadenverursacher und zu den Beteiligten. Die Meldung wird an die zuständige Verrechnungsstelle (Haftpflicht) des KSA übermittelt.*

**05 KSA-Bescheid prüfen und umsetzen**
*Der KSA prüft den Schaden und teilt die Regulierungsentscheidung mit (Anerkennung, Teilregulierung oder Ablehnung). Das Hauptamt prüft den Bescheid. Bei Anerkennung reguliert der KSA den Schaden. Bei Ablehnung prüft das Hauptamt die Rechtsmittel und beteiligt ggf. das Rechtsamt.*

**06 Regress bei grober Fahrlässigkeit prüfen und bescheiden**
*Hat der KSA reguliert und liegt grobe Fahrlässigkeit vor, prüft das Hauptamt den Regress gegen die oder den Beschäftigten nach § 90 NBG (Beamte) oder den Grundsätzen der beschränkten Arbeitnehmerhaftung (Tarifbeschäftigte). Die Personalabteilung (oe-amt-11) beteiligt die oder den Beschäftigten und erlässt einen Regressbescheid. Bei einfacher Fahrlässigkeit entfällt der Regress.*

**07 Zahlung überwachen**
*Bei Regressforderungen überwacht das Hauptamt gemeinsam mit der Kasse (oe-amt-20) den Zahlungseingang. Bei Zahlungsverzug wird gemahnt. Bei Uneinbringlichkeit wird die Forderung niedergeschlagen.*

**08 Vorgang abschließen und aufbewahren**
*Das Hauptamt erstellt einen Abschlussvermerk. Der Vorgang wird nach den gesetzlichen Fristen aufbewahrt: 10 Jahre bei Sachschäden (§ 199 Abs. 3 Nr. 1 BGB), 30 Jahre bei Personenschäden (§ 199 Abs. 2 BGB). Nach Fristablauf wird der Vorgang vernichtet oder gelöscht.*

**Herkunft des Schrittblocks:** abgeleitet aus § 90 NBG, §§ 280, 619a BGB, den Grundsätzen der beschränkten Arbeitnehmerhaftung, der KSA-Satzung und den Verrechnungsgrundsätzen des KSA Hannover, nicht aus einer Ablauferhebung im Hauptamt.