---
id: dstore-schluesselverwaltung
typ: datenspeicher
system: null
name: Schlüsselverwaltung und Schließanlagen
zuständige-einheit: oe-amt-10
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: B
  schutzbedarf: normal
  vertraulichkeitsklasse: intern
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. e
  aufbewahrung:
    frist: fortlaufend
    beginn: bei Ausgabe des Schlüssels
letzte-aktualisierung: '2026-08-10'
tags:
- Schlüssel
- Schließanlage
- Zugangsberechtigung
- Hausrecht
---


# Schlüsselverwaltung und Schließanlagen

## Definition

Daten zur Verwaltung von Schlüsseln und Schließanlagen in der Kommunalverwaltung: Wer hat welchen Schlüssel zu welchen Räumen, wann wurde er ausgegeben, wann zurückgegeben, und wann als verloren gemeldet. Dokumentiert Zugangsberechtigungen, nicht die ausgeführten Zugänge.

## Felder

- Schlüsselempfängerin/Schlüsselempfänger (Name, Kontaktdaten)
- Schlüsselnummer oder Transpondernummer
- Schließplanbezug (Raum, Gebäude, Etage)
- Ausgabedatum und Rückgabedatum
- Verlustmeldung (Datum, Umstände, Ersatz)
- Empfangsbestätigung (Unterschrift oder elektronisch)

## Hinweise

**Angelegt am 2026-08-04** für `vvt-10-027` Schlüsselverwaltung und Schließanlagen.

**Schutzstufe B.** Schlüsseldaten sind nicht frei zugänglich (A scheidet aus), und ein Missbrauch — die Kenntnis, wer Zugang zu welchem Raum hat — beeinträchtigt für sich genommen nicht die gesellschaftliche Stellung oder die wirtschaftlichen Verhältnisse der betroffenen Person (C). Die Information ist aber schutzwürdig, weil sie den Zugang zu Diensträumen und damit zu den darin verarbeiteten Daten dokumentiert.

**Keine Art. 9/10-Daten.** Die Schlüsselverwaltung dokumentiert Zugangsberechtigungen, keine Gesundheitsdaten und keine strafrechtlichen Verurteilungen. Ein verlorener Schlüssel ist ein Sicherheitsvorfall, aber der Verlust selbst ist kein sensibles personenbezogenes Datum der verlierenden Person.

**Abgrenzung.** Nicht zu verwechseln mit Zutrittsprotokollen (wer hat wann welchen Raum betreten) — dieser Speicher dokumentiert nur die Berechtigung, nicht den tatsächlichen Zutritt.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit hoch.** Im Brand- oder Havariefall muss binnen Minuten feststehen, wer Zugang zu welchem Bereich hat und welche Schlüssel ausgegeben sind. Ein verfälschter Bestand führt Rettungskräfte in die Irre; ein nicht abrufbarer verzögert sie.

Zugleich ist der Bestand die Grundlage dafür, dass beim Ausscheiden einer Person alle Schlüssel zurückgefordert werden. Fehlt ein Eintrag, bleibt ein Zugang bestehen, von dem niemand weiß.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei B.** **Identifikations- und interne Verwaltungsdaten.** Name, Kontaktdaten und der Nachweis, dass eine dienstliche Formalie erledigt ist. Die Angaben sind für die betroffene Person nicht belastend; ihre Preisgabe beeinträchtigt weder die gesellschaftliche Stellung noch die wirtschaftlichen Verhältnisse.

**Das gilt ausdrücklich nur für die Datenschutz-Schutzstufe.** Bei `dstore-it-berechtigungsantrag` und `dstore-schluesselverwaltung` liegt die Brisanz in der Informationssicherheit -- beide stehen dort seit dem 2026-08-04 auf hoher Integrität und hoher Verfügbarkeit. Die beiden Maßstäbe messen Verschiedenes, und das ist hier gut zu sehen.

*Sammelvermerk der Durchsicht vom 2026-08-10.*
