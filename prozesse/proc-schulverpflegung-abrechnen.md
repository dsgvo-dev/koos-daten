---
id: proc-schulverpflegung-abrechnen
titel: Schulverpflegung abrechnen
status: aktiv
zustaendigeEinheit: oe-amt-40
zustaendigeRolle: sachbearbeiter
beteiligte:
  - rolle: caterer
    phase: "3,5"
    aufgabe: "Meldung der Mahlzeitenzahlen und Entgegennahme der Abrechnung"
  - rolle: kasse
    phase: "4"
    aufgabe: "Ausführung des SEPA-Lastschrifteinzugs"
daten:
  datenspeicher:
    - id: dstore-personenstammdaten
    - id: dstore-schulbesuch-ausbildungsstatus
    - id: dstore-gemeinschaftliche-mittagsverpflegung
    - id: dstore-bildungs-und-teilhabebedarf
    - id: dstore-sepa-lastschriftmandat
regelungen:
  - "§ 23 NSchG (Schulverpflegung)"
  - "Bildungs- und Teilhabepaket (BuT) — §§ 28, 29 SGB II"
  - "SEPA-Lastschriftmandat (Art. 4 Nr. 14 DSGVO)"
leika_id: ""
ozg_id: ""
letzte-aktualisierung: 2026-08-04
---

# Schulverpflegung abrechnen

## Prozessschritte

**01 Teilnehmer erfassen**
*Anmeldung zur Mittagsverpflegung durch die Erziehungsberechtigten. Erfassung des Kindes, der Schule und des gewünschten Verpflegungsumfangs. Prüfung, ob ein Anspruch auf Leistungen aus dem Bildungs- und Teilhabepaket (BuT) besteht.*

**02 Mahlzeiten buchen**
*Caterer meldet die täglich ausgegebenen Mahlzeiten pro Kind. Abgleich mit der Anmeldung.*

**03 Kosten berechnen**
*Berechnung des monatlichen Kostenbeitrags unter Berücksichtigung der BuT-Förderung. Bei BuT-Berechtigung: Kostenübernahme durch den Leistungsträger, Eigenanteil entfällt.*

**04 SEPA-Lastschrift auslösen**
*Einzug des Eigenanteils per SEPA-Lastschrift von den Erziehungsberechtigten. Das Mandat wird bei der Anmeldung eingeholt.*

**05 Abrechnung an den Caterer**
*Monatliche Abrechnung der Gesamtzahl der Mahlzeiten mit dem Caterer. Überweisung des kommunalen Anteils und der eingesammelten Elternbeiträge.*