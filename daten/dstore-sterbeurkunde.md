---
id: dstore-sterbeurkunde
typ: datenspeicher
system: null
name: Sterbeurkunde
datenkategorie: Standesamt
zuständige-einheit: oe-amt-31
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: PStG
  - gesetz: PStV
  aufbewahrung:
    frist: 30 Jahre
    beginn: prozessabhängig
letzte-aktualisierung: '2026-08-10'
tags:
- Tod
- Urkunde
- Personenstand
- Standesamt
konvertiert-aus: daten1/dtype-sterbeurkunde.md
---



## Beschreibung

Personenstandsdokument über den Tod einer Person.

## Felder

- Name
- Sterbedatum
- Sterbeort
- Todesursache
- Standesamtsnummer

## Rechtsgrundlage

PStG, PStV

## Löschfrist

30 Jahre

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

**Schutzstufe angehoben 2026-08-04: C → D.** Der Speicher führt „Todesursache" als
Feld. Sterbeurkunden enthalten Todesursachen, die Gesundheitsdaten der verstorbenen
Person sind — und mittelbar genetische Informationen für Angehörige. Das
LfD-Konzept nennt Art. 9 als D-Beispiel. Dass der übrige Inhalt einer Sterbeurkunde
(Name, Datum, Ort) für sich genommen C rechtfertigen mag, ändert daran nichts:
das Maximalprinzip (R6) richtet die Stufe nach dem sensibelsten Feld, das in
diesem Speicher anfallen kann. Vorige Einstufung C war eine Voreinstellung.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** An den Vorgang knüpft eine gesetzliche Frist. Ist der Bestand im entscheidenden Zeitraum nicht abrufbar, läuft die Frist gleichwohl -- mit Rechtsfolgen für die Kommune oder die betroffene Person.

**§ 28 PStG verlangt die Anzeige des Sterbefalls am folgenden Werktag**, und § 8 Nds. BestattG bindet die Bestattung an Fristen. Die Sterbeurkunde ist Voraussetzung für beides.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** Die Einstufung wurde am 2026-08-04 bei der Anlage beziehungsweise
Überarbeitung dieses Speichers ausführlich begründet -- siehe die Hinweise oben. Der
Durchgang vom 2026-08-10 hat sie bestätigt und trägt hier nur den Prüfvermerk nach, der bisher
fehlte.

*Der Vermerk ist kein Formalismus: Ohne ihn zählte der Speicher als ungeprüft, und der
Rückstand wies 129 statt der tatsächlich offenen 115 Speicher aus -- allesamt auf Stufe C.*
