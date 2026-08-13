---
id: proc-schadensersatz-fuer-die-kommune-geltend-machen
titel: Schadensersatz für die Kommune geltend machen
status: aktiv
zustaendigeEinheit: oe-amt-66
zustaendigeRolle: ''
beteiligte:
- einheit: oe-amt-20
  aufgabe: ''
- einheit: oe-amt-10
  aufgabe: ''
daten:
  input: []
  output: []
  datenspeicher:
  - id: dstore-personenstammdaten
  - id: dstore-kontaktdaten
  - id: dstore-kfz-daten
  - id: dstore-sicherheitsmangelmeldung
  - id: dstore-rechnungsdaten
  - id: dstore-debitoren-kreditorendaten
  - id: dstore-forderungstitel-vollstreckung
regelungen:
- §§ 823 ff. Bürgerliches Gesetzbuch (BGB) - deliktischer Schadensersatzanspruch
- § 249 BGB - Art und Umfang des Schadensersatzes
- Straßenverkehrsgesetz (StVG) bei Verkehrsunfällen
- Pflichtversicherungsgesetz (PflVG) - Direktanspruch gegen die Haftpflichtversicherung
- §§ 195, 199 BGB - Verjährung
leika_id: null
ozg_id: null
letzte-aktualisierung: '2026-07-29'
---

# Schadensersatz für die Kommune geltend machen

## Zweck

Durchsetzung von Schadensersatzansprüchen **der Kommune als Geschädigter** gegen
Unfallverursacherinnen und Unfallverursacher, Fahrzeughalter und deren
Haftpflichtversicherungen — bei Schäden an Straßen, Lichtsignalanlagen, Beleuchtung,
Schutzeinrichtungen, Bäumen und sonstigem städtischen Eigentum.

**Abgrenzung nach der Anspruchsrichtung:** Wird die Kommune umgekehrt selbst in Anspruch
genommen, ist das ein eigener Vorgang beim Amt 10 —
`proc-schadensfall-bearbeiten-und-regulieren`.

## Prozessschritte

**01 Schadensereignis erfassen**  
*Aufnahme des Schadens durch den Fachdienst, die Straßenmeisterei oder über eine Meldung; Feststellung von Ort, Zeit und Umfang*

**02 Verursacher ermitteln**  
*Auswertung der Unfallmitteilung, der polizeilichen Unfallaufnahme und des Kennzeichens; bei unbekanntem Verursacher Prüfung weiterer Ermittlungsmöglichkeiten*

**03 Halter- und Versicherungsdaten beschaffen**  
*Anfrage der Halterdaten und der Haftpflichtversicherung zur Vorbereitung des Direktanspruchs nach dem PflVG*

**04 Schadenshöhe feststellen**  
*Ermittlung der Wiederherstellungskosten nach § 249 BGB durch Kostenaufstellung, Angebot oder Gutachten*

**05 Forderung anmelden**  
*Geltendmachung gegenüber Verursacher und Versicherung mit Fristsetzung und Nachweisen*

**06 Zahlungseingang überwachen und mahnen**  
*Überwachung des Eingangs bei der Kasse, Mahnung bei Fristablauf*

**07 Beitreibung veranlassen**  
*Bei Zahlungsverweigerung Übergabe an die Rechtsvertretung, gerichtliche Geltendmachung und Vollstreckung*

**08 Vorgang aufbewahren und löschen**  
*Aufbewahrung 10 Jahre ab Anzeige des Schadens, bei anhängigem Verfahren bis zum rechtskräftigen Abschluss; anschließend Löschung*

## Hinweise

*Angelegt am 2026-07-29 für `vvt-66-003`. Die VVT führte bisher drei Prozesse, die alle die
**Meldung** eines Schadens abbilden — die Durchsetzung der Forderung, also der eigentliche
Zweck „Abwicklung von Schadensfällen", war nicht abgebildet.*

**Herkunft des Schrittblocks:** abgeleitet aus dem Anspruchsaufbau der §§ 823, 249 BGB und
dem Inhalt der `vvt-66-003`, nicht aus einer Ablauferhebung im Amt 66.

**Warum die Anspruchsrichtung den Prozess bestimmt.** Betroffene sind hier die
**Unfallverursacher**, nicht die Geschädigten: Es werden Halterdaten beschafft, eine Forderung
angemeldet und notfalls vollstreckt. Bei `proc-schadensfall-bearbeiten-und-regulieren` ist es
umgekehrt — dort werden Bankdaten der Geschädigten verarbeitet, um auszuzahlen. Gleicher
Sachverhalt, entgegengesetzte Datenverarbeitung.

**Keine LeiKa-Nummer:** Die Durchsetzung eigener Forderungen ist keine Leistung gegenüber
Bürgerinnen und Bürgern.
