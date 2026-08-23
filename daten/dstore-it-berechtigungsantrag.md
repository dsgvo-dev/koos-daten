---
id: dstore-it-berechtigungsantrag
name: IT-Berechtigungsantrag
zuständige-einheit: oe-amt-15
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: hoch
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: IT-Sicherheitsrichtlinie der Verwaltung
  aufbewahrung:
    frist: 3 Jahre
    beginn: nach Entzug der Berechtigung
    hinweis: Dokument bleibt während der gesamten Dauer der Berechtigung aufzubewahren
letzte-aktualisierung: '2026-08-10'
---


# IT-Berechtigungsantrag

## Definition

Formular zur Beantragung, Änderung oder zum Entzug von IT-Zugriffsrechten für Beschäftigte
und ggf. externe Personen.

## Typische Inhalte

- Antragstellende Person und genehmigungsberechtigte Führungskraft
- Beantragte Systeme und Zugriffsebenen
- Begründung und ggf. Befristung
- Unterschriften: Antrag, Genehmigung, IT-Administration

## Hinweise

Freigabe erfolgt durch die jeweilige Führungskraft. Die IT-Administration setzt die
Berechtigung erst nach vorliegender Unterschrift um. Änderungen und Entzug folgen dem
gleichen Formularweg.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit hoch.** Der Bestand entscheidet, wer auf welche Fachverfahren zugreifen darf. Eine unbemerkte Verfälschung verschafft Zugriff, der nie beantragt wurde.

Beim Ausscheiden einer Person müssen die Rechte **sofort** entzogen werden -- dafür muss der Bestand vollständig und abrufbar sein. Ein unvollständiges Berechtigungsverzeichnis ist der häufigste Befund bei Prüfungen nach Art. 32 DSGVO.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei B.** **Identifikations- und interne Verwaltungsdaten.** Name, Kontaktdaten und der Nachweis, dass eine dienstliche Formalie erledigt ist. Die Angaben sind für die betroffene Person nicht belastend; ihre Preisgabe beeinträchtigt weder die gesellschaftliche Stellung noch die wirtschaftlichen Verhältnisse.

**Das gilt ausdrücklich nur für die Datenschutz-Schutzstufe.** Bei `dstore-it-berechtigungsantrag` und `dstore-schluesselverwaltung` liegt die Brisanz in der Informationssicherheit -- beide stehen dort seit dem 2026-08-04 auf hoher Integrität und hoher Verfügbarkeit. Die beiden Maßstäbe messen Verschiedenes, und das ist hier gut zu sehen.

*Sammelvermerk der Durchsicht vom 2026-08-10.*
