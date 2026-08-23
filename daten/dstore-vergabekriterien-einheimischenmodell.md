---
id: dstore-vergabekriterien-einheimischenmodell
typ: datenspeicher
system: null
name: Vergabekriterien Wohnbaugrundstücke (Einheimischenmodell)
zuständige-einheit: oe-amt-23
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: normal
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. e
  - gesetz: NKomVG
    artikel: § 125
  - gesetz: NDSG
    artikel: § 3
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Abschluss des Vergabeverfahrens
    hinweis: Bindungsfristen der Vergaberichtlinie und Nachweispflichten gegenüber
      der Kommunalaufsicht; Festlegung des Trägers.
letzte-aktualisierung: '2026-08-04'
tags:
- Grundstücksvergabe
- Einheimischenmodell
- Wohnbauland
---


# Vergabekriterien Wohnbaugrundstücke (Einheimischenmodell)

## Definition

Angaben zur Bewertung von Bewerbungen um städtische Wohnbaugrundstücke nach den Kriterien der kommunalen Vergaberichtlinie.

## Felder

- Bewerbende Person
- Dauer der Ortsbindung (Wohnsitz oder Arbeitsstätte)
- Zahl der im Haushalt lebenden Kinder
- Haushaltseinkommen
- erreichte Punktzahl
- Rangfolge im Vergabeverfahren
- Zu- oder Absage

## Hinweise

Angelegt am 2026-08-03 zu `vvt-23-007` (Vergabe Wohnbaugrundstücke), nach Auskunft des Fachamts vom 2026-08-03.

Die Datenkategorien nannten allein „Name, Adresse" -- obwohl der Zweck ausdrücklich „Vergabekriterien wie Einheimischenmodell" anführt. Ortsbindung, Kinderzahl und Einkommen sind die tragenden Merkmale eines solchen Verfahrens und waren im Verzeichnis nicht abgebildet.

**Die Ortsbindung ist unionsrechtlich heikel.** Der EuGH hat Einheimischenmodelle, die allein an die Ansässigkeit anknüpfen, an der Freizügigkeit gemessen (Urt. v. 08.05.2013, C-197/11 und C-203/11 -- Libert). Die mit der Europäischen Kommission abgestimmten „Neuen Einheimischenmodelle" arbeiten deshalb mit einem Punktesystem aus mehreren sozialen Kriterien statt mit einer Ortsansässigkeitsschwelle. Die erreichte Punktzahl gehört deshalb zur Datenart: Ohne sie ist nicht nachvollziehbar, ob die Auswahl den Vorgaben entspricht.

**Einkommensangaben sind sparsam zu halten.** Für die Punktvergabe genügt regelmäßig eine Einkommensstufe; die Vorlage vollständiger Einkommensnachweise ist dafür nicht erforderlich.

## Schutzstufe geprüft 2026-08-14

**C → D.** Haushaltseinkommen + Zahl der Kinder + Rangfolge/Zu- oder Absage offenbaren die wirtschaftlichen und familiären Verhältnisse der Bewerber um Wohnbaugrundstücke. Das Haushaltseinkommen ist konsistent mit `einkommensdaten` (D). Die Datei selbst dokumentiert, dass Einkommen und Kinderzahl die „tragenden Merkmale" des Einheimischenmodells sind.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*
