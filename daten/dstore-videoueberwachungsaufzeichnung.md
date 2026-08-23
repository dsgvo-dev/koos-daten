---
id: dstore-videoueberwachungsaufzeichnung
typ: datenspeicher
system: null
name: Videoüberwachungsaufzeichnung
zuständige-einheit: oe-amt-23
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
    artikel: § 14
  - gesetz: DSGVO
    artikel: Art. 35 Abs. 3 Buchst. c
  - gesetz: NPersVG
    artikel: §§ 67, 78
  aufbewahrung:
    frist: 10 Tage
    beginn: mit der Aufzeichnung
    hinweis: Festlegung des Trägers. Wird eine Sequenz zur Abwehr einer konkreten
      Gefahr oder zur Verfolgung einer Straftat oder Ordnungswidrigkeit benötigt,
      wird sie vor Fristablauf gesondert gesichert und mit dem Abschluss des Verfahrens
      gelöscht.
letzte-aktualisierung: '2026-08-10'
tags:
- Videoüberwachung
- Sicherheit
- Hausrecht
---



# Videoüberwachungsaufzeichnung

## Definition

Bildaufzeichnungen aus der Videoüberwachung kommunaler Einrichtungen und öffentlich zugänglicher Räume nach § 14 NDSG.

## Felder

- Kamerakennung und Erfassungsbereich
- Aufnahmezeitpunkt
- Bildaufnahme
- Sicherungsvermerk mit Anlass, sobald eine Sequenz aus dem Regelumlauf genommen wird
- Auswertungsvermerk mit Datum, auswertender Person und Anlass
- Übermittlungsvermerk bei Herausgabe an Polizei, Staatsanwaltschaft oder Gericht

## Hinweise

Angelegt am 2026-07-30 zusammen mit `proc-videoueberwachung-betreiben` und `vvt-23-002`.

**Bewusst getrennt von `dstore-bild-und-tonaufnahmen`.** Jener Speicher ist am 2026-07-29 für die Öffentlichkeitsarbeit angelegt worden und führt Einwilligungsstatus und Widerrufsvermerk als Felder. Bei der Videoüberwachung gibt es keine Einwilligung -- die Verarbeitung beruht auf § 14 Abs. 1 NDSG. Ein gemeinsamer Speicher würde eine Rechtsgrundlage suggerieren, die hier nicht besteht, und einen Widerruf nahelegen, den es nicht gibt.

**Der Auswertungsvermerk ist ein Feld, kein Beiwerk.** Im Regelbetrieb wird das laufende Material nicht ausgewertet. Jede Auswertung ist deshalb ein Ereignis, das festgehalten wird -- nur so ist die Beschränkung auf den Anlassfall überprüfbar, und nur so lässt sich gegenüber dem Personalrat belegen, dass keine Verhaltens- oder Leistungskontrolle stattfindet.

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

**C → D.** **Eine Verarbeitung, für die die Datei selbst Art. 35 Abs. 3 Buchst. c DSGVO nennt, kann nicht auf Stufe C stehen.** Die systematische Überwachung öffentlich zugänglicher Bereiche ist datenschutz-folgenabschätzungspflichtig; das setzt ein hohes Risiko voraus.

Das Bild ist eine offene Datenart. Wer aufgenommen wird, gibt unbeabsichtigt Angaben preis, die unter Art. 9 DSGVO fallen: eine Gehhilfe oder ein Verband zeigt den Gesundheitszustand, eine religiöse Kopfbedeckung die Konfession, das Erscheinungsbild die ethnische Herkunft. Erfasst werden zudem Beschäftigte -- deshalb stehen §§ 67, 78 NPersVG in der Datei.

Der Sicherungsvermerk knüpft an einen konkreten Vorfall, der Übermittlungsvermerk an die Herausgabe an Polizei, Staatsanwaltschaft oder Gericht. Spätestens dort steht die Aufnahme im Zusammenhang mit einem Ermittlungsverfahren.
