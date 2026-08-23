---
id: dstore-anlage-buergerupload
typ: datenspeicher
system: null
name: Von Bürgerinnen und Bürgern hochgeladene Anlagen
zuständige-einheit: oe-amt-33
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. e
  - gesetz: NDSG
    artikel: § 3
  - gesetz: NDSG
    artikel: § 17
  aufbewahrung:
    frist: bis zur Übergabe an das Fachverfahren, längstens 30 Tage
    beginn: nach Eingang
    hinweis: Das Portal ist Eingangskanal, nicht Ablage. Nach Übergabe an das zuständige
      Fachverfahren gilt dessen Frist; die Kopie im Portal ist zu löschen.
letzte-aktualisierung: '2026-08-10'
tags:
- Serviceportal
- Upload
- Art. 9 DSGVO
---



# Von Bürgerinnen und Bürgern hochgeladene Anlagen

## Definition

Dateien, die Nutzende einem Anliegen über ein Serviceportal beifügen.

## Felder

- Anliegen und Vorgangsnummer
- Dateiname und Dateityp
- Eingangszeitpunkt
- hochladende Person
- Übergabe an das Fachverfahren mit Datum
- Löschvermerk

## Hinweise

Angelegt am 2026-08-03 zu `vvt-33-006` (Kontaktaufnahme über ServicePortal).

**Stufe D, weil der Inhalt nicht steuerbar ist.** Wie beim Freitextfeld eines Chatbots bestimmt die nutzende Person, was hochgeladen wird -- ein ärztliches Attest, ein Schwerbehindertenausweis, ein Sozialleistungsbescheid, ein Gerichtsbeschluss. Die Verantwortliche kann das nicht verhindern, muss es aber einkalkulieren. Maximalprinzip.

**Die Rechtsgrundlage der Anlage folgt dem Fachverfahren, nicht dem Portal.** Wer ein Attest zu einem Antrag hochlädt, tut das, weil das Fachverfahren es verlangt; dort greift dessen Erlaubnisnorm einschließlich Art. 9 Abs. 2. Das Portal selbst leitet nur weiter. Genau deshalb ist die kurze Frist wesentlich: Solange die Anlage im Portal liegt, wird sie ohne die Grundlage verarbeitet, die sie trägt.

**Praktische Folge:** Übergabe an das Fachverfahren unverzüglich, Löschung der Portalkopie danach, Löschvermerk als Feld.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `normal`** · **Verfügbarkeit: `hoch`**

**Über `normal` gesetzt: Verfügbarkeit `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Integrität bleibt bei `normal`**, geprüft anhand der Fragen des Durchgangs vom 2026-08-04:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** Die Einstufung wurde am 2026-08-04 bei der Anlage beziehungsweise
Überarbeitung dieses Speichers ausführlich begründet -- siehe die Hinweise oben. Der
Durchgang vom 2026-08-10 hat sie bestätigt und trägt hier nur den Prüfvermerk nach, der bisher
fehlte.

*Der Vermerk ist kein Formalismus: Ohne ihn zählte der Speicher als ungeprüft, und der
Rückstand wies 129 statt der tatsächlich offenen 115 Speicher aus -- allesamt auf Stufe C.*
