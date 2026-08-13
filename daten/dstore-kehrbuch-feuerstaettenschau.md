---
id: dstore-kehrbuch-feuerstaettenschau
typ: datenspeicher
system: null
name: Kehrbuch und Feuerstättenschau
datenkategorie: Gewerbe & Erlaubnisse
zuständige-einheit: oe-amt-60
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c und lit. e
  - gesetz: SchfHwG
    artikel: § 14
  - gesetz: SchfHwG
    artikel: § 16
  - gesetz: SchfHwG
    artikel: § 19
  aufbewahrung:
    frist: 7 Jahre
    beginn: nach Ablauf des Kalenderjahres der Eintragung
    hinweis: § 19 Abs. 3 SchfHwG.
letzte-aktualisierung: '2026-08-10'
tags:
- Schornsteinfeger
- Kehrbuch
- Feuerstättenschau
---


# Kehrbuch und Feuerstättenschau

## Definition

Angaben zu Grundstücken und deren Eigentümern im Kehrbuch nach § 16 SchfHwG einschließlich der Ergebnisse der Feuerstättenschau nach § 14 SchfHwG.

## Felder

- Grundstück mit Anschrift
- Eigentümerin oder Eigentümer
- Feuerstätten und Abgasanlagen
- Termine und Ergebnisse der Feuerstättenschau
- Fristsetzungen und Mängel
- Feuerstättenbescheid
- Nachweise über durchgeführte Arbeiten

## Hinweise

Angelegt am 2026-08-03 zu `vvt-60-007` (Schornsteinfegerwesen), nach Auskunft des Fachamts vom 2026-08-03.

**Eine ganze Betroffenengruppe fehlte.** Die VVT zitierte § 16 SchfHwG, führte als Betroffene aber nur die Schornsteinfeger. Im Kehrbuch stehen die Daten der Grundstückseigentümer -- ein deutlich größerer Personenkreis als die Berufsträger, die es führen. Die Betroffenengruppe ist ergänzt worden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit hoch.** Der Bestand dient der Gefahrenabwehr. Ist er verfälscht oder im entscheidenden Moment nicht abrufbar, kann die Kommune ihre Schutzaufgabe nicht erfüllen -- mit möglichen Folgen für Leib und Leben.

Das Kehrbuch dokumentiert Fristen und Mängel an Feuerstätten. Eine übersehene oder verfälschte Frist bedeutet eine nicht geprüfte Feuerstätte.

## Schutzstufe geprüft 2026-08-10

**B → C.** Das Kehrbuch nach § 19 SchfHwG ist zunächst ein Gebäudeverzeichnis. Anzuheben ist es wegen der Felder **Fristsetzungen und Mängel** sowie **Nachweise über durchgeführte Arbeiten**: Sie halten fest, wer einer bauordnungsrechtlichen Pflicht nicht nachgekommen ist.

Bleibt ein Mangel unbeseitigt, folgt die Anordnung der Behörde nach § 5 SchfHwG und im weiteren Verlauf ein Bußgeld nach § 24 SchfHwG. Die Datenart dokumentiert damit ein ordnungswidriges Verhalten -- wenn auch am unteren Rand dessen, was Stufe C trägt.
