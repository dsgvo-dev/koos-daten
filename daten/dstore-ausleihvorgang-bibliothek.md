---
id: dstore-ausleihvorgang-bibliothek
typ: datenspeicher
system: null
name: Ausleihvorgang in der Bibliothek
zuständige-einheit: oe-amt-41
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
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. b
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. e
  - gesetz: NDSG
    artikel: § 3
  - gesetz: NDSG
    artikel: § 17
  aufbewahrung:
    frist: bis zur Rückgabe, danach unverzüglich
    beginn: mit der Rückgabe des Mediums
    hinweis: Nach der Rückgabe besteht kein Zweck mehr für die Zuordnung von Person
      und Medium. Offene Gebührenforderungen sind getrennt zu führen, ohne den Titel
      des Mediums zu nennen.
letzte-aktualisierung: '2026-08-10'
tags:
- Bibliothek
- Ausleihe
- Lesefreiheit
---


# Ausleihvorgang in der Bibliothek

## Definition

Zuordnung entliehener Medien zu einer Nutzerin oder einem Nutzer der öffentlichen Bibliothek.

## Felder

- Nutzerin oder Nutzer mit Ausweisnummer
- entliehenes Medium mit Titel und Signatur
- Ausleihdatum und Rückgabefrist
- Verlängerungen
- Vormerkungen
- Rückgabedatum
- Mahnstufe und Gebühren

## Hinweise

Angelegt am 2026-08-03 zu `vvt-41-001` (Ausleihe von Medien und Nutzerverwaltung öffentliche Bibliothek).

**Die Datenkategorien nannten nur Name, Adresse, Geburtsdatum und Kontaktdaten** -- also die Nutzerverwaltung, nicht die Ausleihe. Dabei ist die Ausleihe der Zweck der Einrichtung, und sie erzeugt die eigentlich schutzbedürftigen Daten.

**Stufe D.** Welche Bücher jemand liest, lässt Rückschlüsse auf religiöse und weltanschauliche Überzeugungen, politische Meinung, Gesundheitszustand und sexuelle Orientierung zu -- ein Ratgeber zu einer Erkrankung, ein Buch über Sucht, Literatur zu einer Glaubensrichtung, ein Titel zur Geschlechtsidentität. Die Zuordnung von Person und Titel ist der Kern des Problems, nicht der einzelne Titel.

Bibliotheken sind für diesen Zusammenhang seit jeher sensibilisiert; die Berufsverbände empfehlen die unverzügliche Löschung der Verknüpfung nach Rückgabe. Genau das ist hier als Frist gesetzt.

**Offene Gebührenforderungen sind getrennt zu führen.** Wird eine Mahnung mit dem Titel des Mediums geführt, bleibt die Verknüpfung über die Rückgabe hinaus bestehen. Für die Forderung genügen Betrag und Vorgangsnummer.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Familiäre, aufenthaltsrechtliche und weltanschauliche Verhältnisse.** Anders als bei den am selben Tag herabgestuften Personenstandsspeichern trägt dieser Bestand eine Angabe, die für sich genommen belastend ist -- eine Sorgerechtsentscheidung, die Abstammung, die Religionszugehörigkeit, den Aufenthaltsstatus oder die Ausübung eines Grundrechts. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
