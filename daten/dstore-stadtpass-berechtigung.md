---
id: dstore-stadtpass-berechtigung
typ: datenspeicher
system: null
name: Stadtpass und Berechtigung
zuständige-einheit: oe-amt-50
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
    artikel: Art. 6 Abs. 1 lit. e
  - gesetz: kommunale Satzung
  aufbewahrung:
    frist: prozessabhängig
    beginn: nach Ablauf der Gültigkeit
    hinweis: Festlegung des Trägers
letzte-aktualisierung: '2026-08-15'
tags:
- Stadtpass
- Vergünstigung
---

# Stadtpass und Berechtigung

## Definition

Daten zur Berechtigung und Ausstellung eines Stadtpasses für vergünstigten Zugang
zu kommunalen Leistungen.

## Felder

- Person
- Berechtigungsgrund
- Gültigkeit
- Ausstellungsdatum

## Schutzstufe geprüft 2026-08-15

**C.** Der Stadtpass ist eine freiwillige kommunale Vergünstigung mit
Einkommensbezug (Berechtigungsprüfung über Einkommensgrenze). C ist angemessen —
keine Art. 9-Daten, Einkommensbezug allein rechtfertigt kein D.

## BSI-Vektoren geprüft 2026-08-15

## Hinweise

**Entwurf aus der Regensburg-Lückenanalyse (2026-08-15).** Freiwillige Leistung der
Kommune. Vor Übernahme in den KOOS-Bestand ist der Fachbereich einzubeziehen und zu
klären, ob der Berechtigungsgrund Einkommensdaten offenbart (dann Schutzstufe D).
