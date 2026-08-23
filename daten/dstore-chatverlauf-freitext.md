---
id: dstore-chatverlauf-freitext
typ: datenspeicher
system: null
name: Chatverlauf mit Freitexteingaben
zuständige-einheit: oe-amt-15
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
    artikel: Art. 6 Abs. 1 lit. e
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. a
  - gesetz: NDSG
    artikel: § 3
  - gesetz: NDSG
    artikel: § 17
  aufbewahrung:
    frist: 30 Tage
    beginn: nach Ende der Konversation
    hinweis: Kurze Frist, weil der Inhalt nicht steuerbar ist. Eine längere Vorhaltung
      vergrößert nur die Menge unkontrolliert mitgeteilter Daten.
letzte-aktualisierung: '2026-08-10'
tags:
- Chatbot
- KI
- Art. 9 DSGVO
- Digitale Verwaltung
---



# Chatverlauf mit Freitexteingaben

## Definition

Von Nutzenden frei eingegebener Text in einem Chatbot der Kommune samt Antworten des Systems.

## Felder

- Konversations-ID
- Zeitpunkt
- Freitexteingaben der nutzenden Person
- Systemantworten
- Bewertung der Antwortqualität
- Weiterleitung an eine Fachstelle, soweit erfolgt

## Hinweise

Angelegt am 2026-08-03 zu `vvt-15-002` (Nutzung des Chatbots).

**Stufe D, weil der Inhalt nicht steuerbar ist.** Bei einem Freitextfeld bestimmt die nutzende Person, was hineingerät. Erfahrungsgemäß werden Anliegen geschildert wie „Ich beantrage Sozialhilfe", „Meine Tochter ist behindert, welche Hilfen gibt es", „Ich werde von meinem Mann bedroht". Das sind Daten nach Art. 9 Abs. 1 DSGVO und teils Angaben, die eine Gefährdungslage offenbaren.

Die Verantwortliche kann das nicht verhindern, aber sie muss es einkalkulieren. Maximalprinzip: Maßgeblich ist, was anfallen **kann**.

**Drei Punkte für die Ausgestaltung:**

1. **Hinweis vor der Eingabe.** Nutzende sind darauf hinzuweisen, keine sensiblen Angaben einzugeben, und auf den regulären Kanal zu verweisen. Das ersetzt die Einstufung nicht, verringert aber das Aufkommen.
2. **Auftragsverarbeitung prüfen.** Läuft das Sprachmodell bei einem Dienstleister, ist ein Vertrag nach Art. 28 DSGVO erforderlich; bei Verarbeitung außerhalb des EWR zusätzlich eine Grundlage nach Kapitel V.
3. **Kein Training mit Verlaufsdaten** ohne eigene Rechtsgrundlage. Die Aufgabenerfüllung nach § 3 NDSG trägt die Beantwortung von Anfragen, nicht die Weiterentwicklung eines Modells.

**Keine automatisierte Entscheidung.** Der Chatbot erteilt Erstinformationen und trifft keine Entscheidung mit rechtlicher Wirkung; Art. 22 DSGVO greift nicht. Das ändert sich, sobald er Anträge vorprüft oder ablehnt.

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
