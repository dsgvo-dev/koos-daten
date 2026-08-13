---
id: proc-rotes-kennzeichen-07er-oldtimer-zuteilen
titel: Rotes Fahrzeugkennzeichen (07er) für Oldtimer zuteilen
status: aktiv
zustaendigeEinheit: oe-amt-34
zustaendigeRolle: ''
beteiligte:
- einheit: oe-amt-20
  aufgabe: ''
daten:
  input: []
  output: []
  datenspeicher:
  - id: dstore-kfz-daten
  - id: dstore-personenstammdaten
  - id: dstore-identitaetsnachweis
  - id: dstore-fuehrungszeugnis
  - id: dstore-bescheinigung
regelungen:
- § 43 Abs. 2 i. V. m. § 41 Abs. 2 Fahrzeug-Zulassungsverordnung (FZV) - Rote Kennzeichen, Zuverlässigkeit
- § 23 Straßenverkehrs-Zulassungs-Ordnung (StVZO) - Oldtimer-Begutachtung
- § 6 Straßenverkehrsgesetz (StVG) - Fahrzeugregister
leika_id: '99036035069000'
ozg_id: null
letzte-aktualisierung: '2026-07-28'
---

# Rotes Fahrzeugkennzeichen (07er) für Oldtimer zuteilen

## Zweck

Zuteilung eines roten Dauerkennzeichens beginnend mit **07** an Halterinnen und Halter
historischer Fahrzeuge. Das Kennzeichen ist einem Fahrzeug nicht fest zugeordnet und kann für
mehrere im Fahrzeugscheinheft eingetragene Oldtimer wechselweise verwendet werden.

**Zulässige Fahrten:** Teilnahme an Veranstaltungen für Oldtimer einschließlich An- und
Abfahrt, Probefahrten sowie Fahrten zu Wartung und Instandsetzung. Alltagsnutzung ist
ausgeschlossen.

**Abgrenzung:** Als einzige der drei roten Kennzeichenarten wird das 07er auch an
**Privatpersonen** erteilt. Das 05er (`proc-rotes-kennzeichen-05er-pruefungsfahrten-zuteilen`)
und das 06er (`proc-rotes-kennzeichen-06er-probe-und-ueberfuehrungsfahrten-zuteilen`) sind
gewerblichen Antragstellern vorbehalten.

## Prozessschritte

**01 Antrag entgegennehmen**  
*Schriftlicher Antrag; persönliche Vorsprache erforderlich*

**02 Oldtimereigenschaft prüfen**  
*Gutachten einer amtlich anerkannten Prüforganisation nach § 23 StVZO; Erstzulassung vor mindestens 30 Jahren, weitgehend originaler Zustand*

**03 Zuverlässigkeit prüfen**  \n*Persönliche Zuverlässigkeit nach § 43 Abs. 2 i. V. m. § 41 Abs. 2 FZV. Auswertung des Führungszeugnisses (Belegart O) und ggf. Auskunft aus dem Fahreignungsregister.*

**04 Versicherungsnachweis prüfen**  
*Bestätigung einer Haftpflichtversicherung für rote Kennzeichen*

**05 Kennzeichen zuteilen und Fahrzeugscheinheft ausgeben**  
*Zuteilung des 07er-Kennzeichens, Eintragung der Fahrzeuge in das Fahrzeugscheinheft*

**06 Dokumentation und Gebührenerhebung**  
*Aufnahme in den Bestand, Gebührenbescheid*

## Hinweise

*Angelegt am 2026-07-28 (Einzelfehler 6). Entstanden aus der Aufteilung von
`proc-rotes-kennzeichen-beantragen`, das alle drei roten Kennzeichenarten in einer Datei
zusammenfasste, obwohl der Katalog sie in drei Leistungsobjekte trennt.*

**Herkunft des Schrittblocks:** abgeleitet aus der Rechtslage und den veröffentlichten
Leistungsbeschreibungen anderer Zulassungsbehörden, nicht aus einer Ablauferhebung im Amt 34.
Der Datenspeicher `dstore-fuehrungszeugnis` ist neu aufgenommen — die Zuverlässigkeitsprüfung
war in der Ursprungsdatei nicht abgebildet.
