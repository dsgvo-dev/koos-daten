---
# Muster Verarbeitungstätigkeit (Art. 30 DSGVO). Datei kopieren nach vvt/vvt-<amt>-<nr>.md und alle <Platzhalter> ersetzen.
# Kommentarzeilen (#) vor dem Speichern entfernen.
id: vvt-<amt>-<nr>
# <amt> = Amtsnummer aus orga.yaml (z. B. 10, 1-5), <nr> = nächste freie dreistellige Nummer des Amtes.
uid: <amt>-<nr>
titel: <Bezeichnung der Verarbeitung>
status: aktiv
# aktiv | inaktiv. „aktiv" heißt: wird geführt.
organisationseinheit: oe-<id>
zweck: <Zweck der Verarbeitung in einem Satz>
rechtsgrundlage: '<Art. 6 Abs. 1 lit. … DSGVO i. V. m. Fachnorm; bei Beschäftigten Art. 88 DSGVO, § 12 NDSG, § 88 NBG; bei einer Dienstvereinbarung: Ausgestaltung durch die Dienstvereinbarung <Name> (`reg-<id>`) als Kollektivvereinbarung nach § 78 NPersVG, deren Abschluss auf der Mitbestimmung nach § 67 Abs. 1 Nr. 2 NPersVG beruht>'
kategorien_betroffener: <Gruppen, durch Semikolon getrennt>
kategorien_daten: <Datenkategorien, durch Semikolon getrennt>
kontextprofil:
  verfahren-vertraulich: false
  # true, wenn schon die Tatsache, im Verfahren geführt zu werden, der Person schaden kann (regeln/kontextregeln.yaml, Punkt 1).
  # Bei true zusätzlich: fallgruppe: <aus kontextregeln.yaml> und begruendung: <Satz>
  entscheidung: '<JJJJ-MM-TT>'
  regelquelle: regeln/kontextregeln.yaml
datenspeicher:
- id: dstore-<id>
empfaenger: <Empfänger intern und extern; Auftragsverarbeiter mit Art. 28 DSGVO>
transfer_drittland: Nein
# Bei Ja: Drittland, Übermittlungsgrundlage (Art. 45 oder Art. 46 DSGVO) und Umfang.
loeschfrist: <Jede Frist mit Dauer, Beginn und Rechtsgrundlage. Keine Aufgaben („ist festzulegen"), nur Fristen.>
tom: []
# Nicht pflegen. Die Maßnahmen werden in tom/tom-<vvt-id>.json erzeugt.
leika_id: null
ozg_id: null
software_verarbeitungsmittel: <Art des Verfahrens; Herstellernamen nur, wenn das Produkt selbst Gegenstand ist>
prozesse:
- proc-<id>
letzte-aktualisierung: '<JJJJ-MM-TT>'
---

# <Bezeichnung der Verarbeitung>

## Zweck

<Zweck wie im Kopf.>

## Verknüpfte Prozesse

- `proc-<id>`: <Titel>

## Verknüpfte Regelungen

- `reg-<id>`: <Name> — <was die Regelung für diese Verarbeitung festlegt>

## Abgrenzung

<Nur bei Überschneidung: welche benachbarte VVT was führt.>

## Hinweise

**Neuanlage <JJJJ-MM-TT>.** <Anlass.>
