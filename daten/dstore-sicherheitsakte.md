---
id: dstore-sicherheitsakte
bereich: intern
typ: datenspeicher
system: null
name: Sicherheitsakte
zuständige-einheit: oe-amt-10
personenbezug: ja
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c, Art. 9 Abs. 2 lit. g, Art. 10
  - gesetz: Nds. SÜG
    artikel: § 6 Abs. 2, § 13 Abs. 2, § 15 Abs. 1, § 16 Abs. 1
  aufbewahrung:
    frist: 1 Jahr nach Abschluss der Überprüfung ohne Aufnahme der Tätigkeit; sonst 5 Jahre nach Ausscheiden aus der sicherheitsempfindlichen Tätigkeit
    beginn: siehe Frist
    hinweis: '§ 16 Abs. 1 Nds. SÜG; mit Einwilligung spätestens 10 Jahre nach diesen Zeitpunkten; keine Vernichtung, solange ein Verwaltungsstreit- oder Strafverfahren nach § 16 Abs. 1 Satz 3 anhängig ist.'
letzte-aktualisierung: '2026-10-05'
tags:
- Sicherheitsüberprüfung
- Nds. SÜG
---

# Sicherheitsakte

## Definition

Sicherheitsakte der zuständigen Stelle nach § 15 Abs. 1 Nds. SÜG über Personen, die mit einer sicherheitsempfindlichen Tätigkeit betraut werden sollen. Zu führen von einer von der Personalverwaltung personell und organisatorisch getrennten Stelle (§ 6 Abs. 2 Nds. SÜG).

## Felder

- betroffene Person (Stammdaten)
- Art der Überprüfung und sicherheitsempfindliche Tätigkeit
- Sicherheitserklärung
- Verlauf und Abschluss der Überprüfung
- Mitteilungen nach § 13 Abs. 2 Satz 2 Nds. SÜG (Umsetzung, Versetzung, Ausscheiden; Änderungen von Familienstand, Name, Wohnsitz, Staatsangehörigkeit; Anhaltspunkte für Abhängigkeiten oder Überschuldung; Straf- und Disziplinarsachen)

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). vvt-10-029 nutzte bis dahin `dstore-personenstammdaten-vertraulich`, `dstore-zuverlaessigkeitsanfrage-sicherheitsbehoerden` und `dstore-register-und-zuverlaessigkeitsauskuenfte`, alle extern. Die Anfragen bei Behörden stellt nach § 9 Abs. 3 Nds. SÜG die mitwirkende Behörde (Verfassungsschutz); sie gehören nicht in die Akte der Kommune.

**Schutzstufe D.** Enthält Angaben zu Abhängigkeiten (Art. 9), Straf- und Disziplinarsachen (Art. 10) und Überschuldung.

**BSI-Vektoren.** Vertraulichkeit hoch, Integrität hoch, Verfügbarkeit normal — Vertraulichkeit hoch; Integrität hoch, weil die Akte Grundlage der Entscheidung über den Einsatz ist.

**Abgrenzung:**
- `dstore-sicherheitserkenntnisse`: Ergebnis und Erkenntnisse der mitwirkenden Behörde.
- `dstore-personalakte`: nach § 6 Abs. 2 Nds. SÜG von der Sicherheitsakte getrennt.
