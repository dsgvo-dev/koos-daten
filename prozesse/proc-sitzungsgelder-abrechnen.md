---
id: proc-sitzungsgelder-abrechnen
titel: Sitzungsgelder und Entschädigungen der Vertretung abrechnen
status: aktiv
zustaendigeEinheit: oe-amt-10
zustaendigeRolle: ''
beteiligte:
- einheit: oe-amt-20
  aufgabe: ''
- einheit: oe-amt-11
  aufgabe: ''
daten:
  input: []
  output: []
  datenspeicher:
  - id: dstore-personenstammdaten
  - id: dstore-kontaktdaten
  - id: dstore-bankverbindung
  - id: dstore-steuerdaten
  - id: dstore-abrechnungsdaten
  - id: dstore-sitzungsprotokoll
  - id: dstore-ehrenamtsdaten
regelungen:
- § 55 Abs. 1 Satz 1 NKomVG - Anspruch der Abgeordneten auf Entschädigung nach § 44 Abs. 1 und 3
- § 44 Abs. 1 NKomVG - Ersatz der Auslagen einschließlich Kinderbetreuungskosten und des nachgewiesenen Verdienstausfalls
- § 44 Abs. 3 NKomVG - Stundenpauschale für Personen ohne Verdienstausfall
- § 55 Abs. 2 NKomVG - Empfehlungen der Entschädigungskommission
- Entschädigungssatzung der Kommune - Ausgestaltung und Höhe
- Art. 6 Abs. 1 lit. b) DSGVO - Vergütung von Referierenden und Sachverständigen auf vertraglicher Grundlage
- § 3 Nr. 12 EStG - Steuerfreiheit von Aufwandsentschädigungen; §§ 38 ff. EStG für steuerpflichtige Bestandteile
- § 147 AO und NKomHKVO - Aufbewahrung
leika_id: null
ozg_id: null
letzte-aktualisierung: '2026-07-29'
---

# Sitzungsgelder und Entschädigungen der Vertretung abrechnen

## Zweck

Berechnung, Festsetzung und Auszahlung der Entschädigung der Abgeordneten und der
Ausschussmitglieder: Sitzungsgeld, Aufwandsentschädigung, Ersatz von Auslagen und
Kinderbetreuungskosten, Ersatz des nachgewiesenen Verdienstausfalls, Fahrtkosten. Umfasst
zugleich die Vergütung von Referierenden und Sachverständigen auf vertraglicher Grundlage.

**Abgrenzung:** Das Sitzungsmanagement selbst — Einladung, Vorlagen, Niederschrift — ist
`vvt-10-014`. Dieser Prozess setzt auf den dort erzeugten Teilnahmenachweisen auf.

## Prozessschritte

**01 Teilnahme feststellen**  
*Übernahme der Anwesenheit aus den Sitzungsniederschriften je Gremium, Datum und Dauer*

**02 Anspruch nach der Entschädigungssatzung ermitteln**  
*Zuordnung von Sitzungsgeld, Aufwandsentschädigung und Funktionszuschlägen nach der Entschädigungssatzung*

**03 Verdienstausfall und Auslagen prüfen**  
*Prüfung der eingereichten Nachweise über Verdienstausfall, Kinderbetreuungskosten und Fahrtkosten nach § 44 Abs. 1 NKomVG; bei Selbständigen erleichterter Nachweis, für Personen ohne Verdienstausfall die Stundenpauschale nach § 44 Abs. 3 NKomVG*

**04 Steuerpflicht der Bestandteile bestimmen**  
*Trennung der steuerfreien Aufwandsentschädigung im Rahmen des § 3 Nr. 12 EStG von den steuerpflichtigen Bestandteilen, insbesondere dem Verdienstausfallersatz*

**05 Steuer-ID nur für steuerpflichtige Bestandteile erheben**  
*Anforderung der Steuer-Identifikationsnummer ausschließlich bei den Personen, bei denen steuerpflichtige Bestandteile anfallen*

**06 Vergütung von Referierenden und Sachverständigen abrechnen**  
*Abrechnung auf Grundlage der geschlossenen Vergütungsvereinbarung, nicht nach der Entschädigungssatzung*

**07 Auszahlung anordnen**  
*Auszahlungsanordnung an die Kasse auf die hinterlegte Bankverbindung*

**08 Lohnsteuer anmelden**  
*Meldung der steuerpflichtigen Bestandteile an das Finanzamt*

**09 Unterlagen aufbewahren und löschen**  
*Aufbewahrung 10 Jahre nach der NKomHKVO und, für die steuerlich erheblichen Unterlagen, nach § 147 AO; anschließend Löschung*

## Hinweise

*Angelegt am 2026-07-29 für `vvt-10-015`.*

**Herkunft des Schrittblocks:** abgeleitet aus der Normenkette des § 55 i. V. m. § 44 NKomVG
und dem Steuerrecht, nicht aus einer Ablauferhebung im Amt 10.

**Zwei Personengruppen, zwei Rechtsgrundlagen.** Das ist der Grund für den eigenen Schritt 06:

| Gruppe | Grundlage | Charakter |
|---|---|---|
| Abgeordnete, Ausschussmitglieder, sachkundige Bürgerinnen und Bürger, entsandte Vertretende | § 55 Abs. 1 Satz 1 i. V. m. § 44 Abs. 1 und 3 NKomVG, **Entschädigungssatzung** | gesetzlicher Anspruch, Art. 6 Abs. 1 lit. e DSGVO |
| Referierende und Sachverständige mit Vergütungsvereinbarung | **Vertrag**, Art. 6 Abs. 1 lit. b) DSGVO | keine Entschädigung nach NKomVG |

Die Entschädigungssatzung trägt nur die erste Gruppe. Für die zweite ist der Vertrag die
Grundlage — sie erhalten keine Entschädigung, sondern eine Vergütung.

**Die Steuer-ID wird nicht pauschal erhoben** (Schritte 04 und 05). Aufwandsentschädigungen
sind im Rahmen des § 3 Nr. 12 EStG steuerfrei; steuerpflichtig ist insbesondere der Ersatz des
Verdienstausfalls. Nur wo steuerpflichtige Bestandteile anfallen, ist die
Steuer-Identifikationsnummer erforderlich. Bei allen übrigen wird sie nicht angefordert.

**Zur Aufbewahrung:** Zehn Jahre bleiben, die Begründung ist berichtigt. Maßgeblich sind die
**NKomHKVO** und für die steuerlich erheblichen Unterlagen § 147 AO. § 257 HGB gilt für
Kaufleute und ist auf die Kommune nicht anwendbar.

**Keine LeiKa-Nummer:** interne Abrechnung, keine Leistung des Leistungskatalogs.
