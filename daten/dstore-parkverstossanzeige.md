---
id: dstore-parkverstossanzeige
typ: datenspeicher
system: null
name: Parkverstoßanzeige
zuständige-einheit: oe-amt-34
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
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: StVO
  - gesetz: OWiG
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Verfahrensabschluss
    hinweis: Fach- und verfahrensabhängig; aus Serviceportal-Kontext abgeleitet
letzte-aktualisierung: '2026-08-10'
tags:
- Parkverstoß
- Anzeige
- Kennzeichen
---


# Parkverstoßanzeige

## Definition

Daten zu gemeldeten Parkverstößen im öffentlichen Verkehrsraum.

## Felder

- Kennzeichen
- Ort
- Zeitpunkt
- Verstoßart
- Fotobeleg
- Meldende Person

## Hinweise

Die Zuständigkeit wurde auf reale `oe-*`-IDs aus `orga.yaml` normalisiert.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-10

**C → D.** Der Verstoß selbst ist eine Bagatelle. **Zwei andere Umstände tragen die Einstufung:**

1. Kennzeichen, Ort, Zeitpunkt und Fotobeleg ergeben zusammen ein **Bewegungsdatum** -- die Feststellung, dass ein bestimmtes Fahrzeug zu einer bestimmten Zeit an einem bestimmten Ort stand. In der Summe mehrerer Anzeigen entsteht daraus ein Bewegungsbild.
2. Das Feld **meldende Person** ist gegenüber dem Betroffenen schutzbedürftig. Anzeigen aus dem ruhenden Verkehr kommen häufig aus der Nachbarschaft; wird die Identität bekannt, kann das einen Konflikt eskalieren lassen. Die Akteneinsicht des Betroffenen nach § 49 OWiG macht diese Frage praktisch relevant.
