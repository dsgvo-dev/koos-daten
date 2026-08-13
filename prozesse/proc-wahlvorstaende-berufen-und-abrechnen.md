---
id: proc-wahlvorstaende-berufen-und-abrechnen
titel: Wahlvorstände berufen und abrechnen
status: aktiv
zustaendigeEinheit: oe-amt-10
zustaendigeRolle: ''
beteiligte:
- einheit: oe-amt-20
  aufgabe: ''
daten:
  input: []
  output: []
  datenspeicher:
  - id: dstore-personenstammdaten
  - id: dstore-kontaktdaten
  - id: dstore-bankverbindung
  - id: dstore-wahlunterlagen
  - id: dstore-ehrenamtsdaten
regelungen:
- § 9 Bundeswahlgesetz (BWahlG) - Wahlvorstände, § 11 Bundeswahlordnung (BWO) - Ehrenamtliche Tätigkeit
- § 78 Europawahlordnung (EuWO)
- § 25 Abs. 3 Niedersächsisches Landeswahlgesetz (NLWG)
- § 11 Abs. 3 und 4 Niedersächsisches Kommunalwahlgesetz (NKWG)
leika_id: null
ozg_id: null
letzte-aktualisierung: '2026-07-29'
---

# Wahlvorstände berufen und abrechnen

## Zweck

Gewinnung, Berufung, Schulung und Abrechnung der Mitglieder der Wahlvorstände
(Wahlhelferinnen und Wahlhelfer) für alle allgemeinen Wahlen. Die Mitwirkung im Wahlvorstand
ist ein **Ehrenamt**; die Gemeinde darf hierfür Beschäftigte des öffentlichen Dienstes und
Wahlberechtigte aus dem Gemeindegebiet heranziehen.

**Abgrenzung:** Die Wahlorganisation im Übrigen — Wahlvorschläge, Wahlausschuss, Wahltag,
Ergebnisfeststellung — ist `proc-wahl-organisieren-und-durchfuehren`.

## Prozessschritte

**01 Bedarf ermitteln**  
*Ermittlung der Zahl der benötigten Wahlvorstandsmitglieder je Wahlbezirk und Briefwahlvorstand*

**02 Wahlhelferinnen und Wahlhelfer gewinnen**  
*Aufruf, Rückgriff auf die Datei früherer Wahlhelfender, Heranziehung von Beschäftigten des öffentlichen Dienstes*

**03 Verfügbarkeit und Wahlberechtigung prüfen**  
*Abgleich der Wahlberechtigung, Prüfung von Ablehnungsgründen und Verfügbarkeit am Wahltag*

**04 Berufung aussprechen**  
*Schriftliche Berufung in den Wahlvorstand mit Angabe von Wahlraum, Funktion und Dienstzeit*

**05 Schulung durchführen**  
*Unterweisung zu Ablauf, Auszählung und Niederschrift*

**06 Einsatz am Wahltag dokumentieren**  
*Erfassung der tatsächlich geleisteten Mitwirkung und der Anwesenheit*

**07 Erfrischungsgeld auszahlen**  
*Festsetzung und Auszahlung des Erfrischungsgeldes beziehungsweise der Aufwandsentschädigung über die Bankverbindung*

**08 Einwilligung für die Wahlhelferdatei einholen**  
*Abfrage, ob die Person für künftige Wahlen erneut angesprochen werden darf; schriftliche oder elektronische Einwilligung nach Art. 6 Abs. 1 lit. a) DSGVO mit Hinweis auf den jederzeitigen Widerruf*

**09 Daten aufbewahren, löschen und Widerruf umsetzen**  
*Aufbewahrung der Wahlunterlagen nach der jeweiligen Wahlordnung; Fortführung der Wahlhelferdatei nur für Personen mit gültiger Einwilligung; sofortige Löschung des Eintrags bei Widerruf*

## Hinweise

*Angelegt am 2026-07-29 für `vvt-10-001` (Europawahl), `vvt-10-006` (Bundestagswahl),
`vvt-10-007` (Landtagswahl) und `vvt-10-008` (Kommunalwahl). Alle vier verweisen auf diesen
Prozess.*

**Herkunft des Schrittblocks:** abgeleitet aus dem gesetzlichen Auftrag der Wahlordnungen,
nicht aus einer Ablauferhebung im Amt 10.

**Warum getrennt von der Wahldurchführung:** Die Wahlvorstandsmitglieder sind ein eigener
Betroffenenkreis, und die Auszahlung des Erfrischungsgeldes verarbeitet mit der
**Bankverbindung** eine Datenart, die in der übrigen Wahlorganisation nicht anfällt.

**Zwei Rechtsgrundlagen in einem Prozess.** Die Schritte 01 bis 07 beruhen auf der
Wahlrechtspflicht (Art. 6 Abs. 1 lit. c DSGVO i. V. m. § 9 BWahlG und den entsprechenden
Landesnormen): Wer herangezogen wird, ist zur Mitwirkung verpflichtet, eine Einwilligung ist
weder erforderlich noch möglich.

Die **Wahlhelferdatei** in den Schritten 08 und 09 ist etwas anderes. Sie dient dazu, bewährte
Wahlhelfende bei der **nächsten** Wahl erneut anzusprechen — das ist von der Pflichtaufgabe
der laufenden Wahl nicht mehr gedeckt und beruht ausschließlich auf der **Einwilligung nach
Art. 6 Abs. 1 lit. a) DSGVO**. Folgen daraus:

- Die Einwilligung ist **freiwillig**: Ihre Verweigerung darf keinen Einfluss auf die
  Heranziehung zur aktuellen Wahl haben.
- Sie ist **jederzeit widerruflich**; der Widerruf führt zur sofortigen Löschung des Eintrags.
- Gespeichert wird nur, was die erneute Ansprache erfordert: Name, Anschrift, Kontaktdaten
  und bisherige Funktion. **Bankverbindungen gehören nicht in die Wahlhelferdatei** — sie
  werden für jede Wahl neu erhoben und nach Ablauf der Wahlordnungsfrist gelöscht.

**Keine LeiKa-Nummer:** interner Organisationsvorgang, keine Leistung gegenüber Bürgerinnen
und Bürgern.
