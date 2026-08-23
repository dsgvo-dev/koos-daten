---
id: dstore-abschleppmassnahme
typ: datenspeicher
system: null
name: Abschleppmaßnahme
zuständige-einheit: oe-amt-32
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: NPOG
    artikel: § 26
  - gesetz: Nds. VwVG
    artikel: § 66
  aufbewahrung:
    frist: 6 Jahre
    beginn: nach Abschluss der Kostenerhebung
    hinweis: Vollstreckungs- und Rechtsbehelfsfristen; Festlegung des Trägers.
letzte-aktualisierung: '2026-08-12'
tags:
- Abschleppen
- Ordnungsrecht
---


# Abschleppmaßnahme

## Definition

Dokumentation einer Abschleppmaßnahme unabhängig davon, ob das Fahrzeug anschließend in Verwahrung genommen wird.

## Felder

- Amtliches Kennzeichen
- Halterin oder Halter
- Standort des Fahrzeugs vor der Maßnahme
- Zeitpunkt der Feststellung und der Abschleppung
- Grund der Maßnahme
- anordnende Person
- beauftragtes Abschleppunternehmen
- Abstellort
- Kosten

## Hinweise

Angelegt am 2026-08-03 zu `vvt-32-007` (Abschleppen von Fahrzeugen).

`dstore-verwahrgut-sicherstellung` führt Verwahrort und Zeitpunkt der Sicherstellung und deckt damit nur den Fall ab, in dem das Fahrzeug nach § 26 NPOG in Verwahrung genommen wird. Beim Abschleppen im Wege der Ersatzvornahme entsteht keine Verwahrung, wohl aber eine dokumentierte Maßnahme mit Standort, Zeitpunkt und Kosten.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-12

**Bleibt bei C.** Der Speicher nennt den Grund der Maßnahme, die anordnende Person und die Kosten. Das Abschleppen folgt regelmäßig einem Parkverstoß; das LfD-Schutzstufenkonzept führt **Ordnungswidrigkeiten** ausdrücklich als Beispiel der Stufe C.

**Nicht D.** Es geht um einen Bagatellvorgang ohne Bezug zur wirtschaftlichen Existenz.

*Durchsicht Los 1 (Amt 32) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los1-amt32.md`.*
