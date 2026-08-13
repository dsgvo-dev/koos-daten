---
id: dstore-bauzeichnungen
typ: datenspeicher
system: null
name: Bauzeichnungen und Baubeschreibung
datenkategorie: Verwaltungsformular
zuständige-einheit: oe-amt-63
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
  - gesetz: NBauO
    artikel: §63 i.V.m. BauVorlVO
    titel: Bauvorlagenverordnung Niedersachsen
  aufbewahrung:
    frist: 10 Jahre nach Abschluss des Verfahrens
    beginn: nach Bestandskraft des Bescheids
    hinweis: Bestandteil der Bauakte; ggf. dauerhaft als bautechnischer Nachweis
letzte-aktualisierung: '2026-08-10'
---


# Bauzeichnungen und Baubeschreibung

## Definition

Technische Unterlagen, die das Bauvorhaben maßstabsgetreu und vollständig darstellen.
Sie sind Pflichtbestandteil jedes Bauantrags nach der Bauvorlagenverordnung (BauVorlVO)
und bilden die Prüfungsgrundlage für die Bauaufsichtsbehörde.

## Typische Inhalte

- Lageplan (amtlich oder nicht-amtlich, je nach Verfahren)
- Grundrisse aller Geschosse (Maßstab 1:100)
- Ansichten und Schnitte (Maßstab 1:100)
- Baubeschreibung (Nutzung, Konstruktion, Materialien)
- Nachweise zu Standsicherheit, Brandschutz, Schallschutz (je nach Verfahren)

## Hinweise

Die Unterlagen müssen von einer bauvorlagenberechtigten Person unterschrieben sein.
Bei vereinfachten Verfahren (§ 63 NBauO) sind Nachweise zu Standsicherheit und Brandschutz
durch die Bauherrin / den Bauherrn eigenverantwortlich zu erbringen.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*

## Schutzstufe geprüft 2026-08-10

**B → C.** Die Bau-Grunddaten sind mehr als Sachdaten.

Grundrisse zeigen die Aufteilung einer Wohnung mitsamt Fenstern, Türen und Zugängen -- eine Angabe, die bei Offenlegung das Einbruchsrisiko erhöht. Bauvorlagen zum barrierefreien Umbau lassen zudem eine Behinderung oder Pflegebedürftigkeit erkennen.

**Kohärenz:** `dstore-bauakte` steht seit dem 2026-08-10 auf Stufe D, weil sie die Nachbareinwendung aufnimmt. Die Einzelbestandteile tragen diese Stufe nicht -- sie tragen aber auch nicht mehr die Stufe B, die sie aus dem Import mitgebracht hatten.
