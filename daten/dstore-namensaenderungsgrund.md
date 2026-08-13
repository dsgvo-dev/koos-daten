---
id: dstore-namensaenderungsgrund
typ: datenspeicher
system: null
name: Begründung einer Namensänderung
datenkategorie: Personenstand & Namensrecht
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
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c
  - gesetz: NamÄndG
    artikel: § 3
  - gesetz: NDSG
    artikel: § 3
  aufbewahrung:
    frist: 30 Jahre
    beginn: nach Bestandskraft der Entscheidung
    hinweis: Die Namensänderung wirkt lebenslang; die Begründung muss für Rückfragen
      und Rechtsbehelfe nachvollziehbar bleiben.
letzte-aktualisierung: '2026-08-10'
tags:
- Namensrecht
- NamÄndG
- Personenstand
---



# Begründung einer Namensänderung

## Definition

Die von der antragstellenden Person vorgetragenen persönlichen Gründe für eine öffentlich-rechtliche Namensänderung sowie die Ergebnisse der Anhörung Dritter.

## Felder

- Antragstellende Person
- alter und neuer Name
- vorgetragener wichtiger Grund nach § 3 NamÄndG
- beigefügte Nachweise
- angehörte Dritte und deren Stellungnahme
- Entscheidung mit Datum

## Hinweise

Angelegt am 2026-08-03 zu `vvt-31-001` (Namensänderungsverfahren), nach Auskunft des Fachamts vom 2026-08-03: Die Begründung besteht in der Regel aus persönlichen Gründen.

**Stufe C, nicht D -- mit einem Vorbehalt für den Einzelfall.** Persönliche Gründe wie ein anstößiger oder schwer aussprechbarer Name beeinträchtigen bei unsachgemäßer Handhabung die gesellschaftliche Stellung, nicht die Existenz. Wird die Änderung jedoch mit **Gewaltschutz, Verfolgung oder einem Gesundheitszustand** begründet, liegen Daten nach Art. 9 Abs. 1 DSGVO vor. Dann ist der Vorgang im Einzelfall wie Stufe D zu behandeln und die Verarbeitung zusätzlich auf Art. 9 Abs. 2 lit. g) DSGVO zu stützen.

Diese Unterscheidung lässt sich nicht am Speicher festmachen, sondern nur am Einzelfall. Sie gehört deshalb in die Bearbeitungshinweise des Fachdienstes.

**Die Anhörung Dritter ist Teil der Datenart.** Nach § 3 NamÄndG sind Personen zu hören, deren Rechte berührt sind -- deren Stellungnahmen enthalten Angaben über die antragstellende Person aus fremder Feder.

## Einstufung nach dem Maximalprinzip 2026-08-03

Die Schutzstufe richtet sich nach der sensibelsten Angabe, die in diesem Speicher anfallen **kann** -- nicht nach dem Regelfall. Ist die Verarbeitung von Daten nach Art. 9 Abs. 1 DSGVO möglich, gilt für den Speicher insgesamt die höhere Stufe.

Der Grund ist praktischer Natur: Technische und organisatorische Maßnahmen werden für den Speicher eingerichtet, nicht für den einzelnen Datensatz. Eine Einstufung, die erst im Einzelfall angehoben wird, führt zu Maßnahmen, die im Einzelfall nicht greifen.

**Von C auf D.** Wird eine Namensänderung mit Gewaltschutz, Verfolgung oder einem Gesundheitszustand begründet, enthält die Begründung Daten nach Art. 9 Abs. 1 DSGVO. Das ist kein seltener Ausnahmefall -- der Schutz vor einer nachstellenden Person ist ein typischer wichtiger Grund nach § 3 NamÄndG. Der zuvor formulierte Einzelfallvorbehalt entfällt; die Verarbeitung ist zusätzlich auf Art. 9 Abs. 2 lit. g) DSGVO zu stützen, sobald solche Gründe vorgetragen werden.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `hoch`** · **Verfügbarkeit: `normal`**

**Über `normal` gesetzt: Integrität `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Verfügbarkeit bleibt bei `normal`**, geprüft anhand der Fragen des Durchgangs vom 2026-08-04:

1. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

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
