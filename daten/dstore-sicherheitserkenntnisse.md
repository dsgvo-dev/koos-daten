---
id: dstore-sicherheitserkenntnisse
typ: datenspeicher
system: null
name: Sicherheitserkenntnisse (Sicherheitsüberprüfung)
zuständige-einheit: oe-amt-10
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: sehr hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: sehr hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: sehr hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 10
  - gesetz: SÜG
    artikel: §§ 2, 3
  aufbewahrung:
    frist: 5 Jahre
    beginn: nach Abschluss des Verfahrens
    hinweis: Festlegung des Trägers; bei Ü2/Ü3 ggf. strenger
letzte-aktualisierung: '2026-08-15'
tags:
- Sicherheitsüberprüfung
- Sicherheitserkenntnisse
- Art. 10
---

# Sicherheitserkenntnisse (Sicherheitsüberprüfung)

## Definition

Sicherheitserhebliche Erkenntnisse über zu überprüfende Personen, die im Rahmen
einer Sicherheitsüberprüfung nach dem Sicherheitsüberprüfungsgesetz von den
Sicherheitsbehörden erhoben und bewertet werden.

## Felder

- Betroffene Person
- Erkenntnis
- Quelle (Behörde)
- Überprüfungsart (Ü1–Ü3)
- Bewertung

## Schutzstufe geprüft 2026-08-15

**D/E (Art. 10).** Sicherheitserhebliche Erkenntnisse können Daten über
strafrechtliche Verurteilungen und Straftaten (Art. 10 DSGVO) sowie
sicherheitsrelevante Bewertungen der Verfassungsschutzbehörden umfassen.
Die Schutzstufe richtet sich nach der Überprüfungsart (Ü1=C/D, Ü2=D, Ü3=E).
Einstweilen D als Mindeststufe gesetzt; Fachbereich muss finale Stufe festlegen.

## BSI-Vektoren geprüft 2026-08-15
