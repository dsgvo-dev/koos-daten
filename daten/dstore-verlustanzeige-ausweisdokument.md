---
id: dstore-verlustanzeige-ausweisdokument
typ: datenspeicher
system: null
name: Verlustanzeige Ausweisdokument
zuständige-einheit: oe-amt-33
bpmn:
  typ: nachricht
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: PAuswG
  - gesetz: PassG
  aufbewahrung:
    frist: prozessabhängig
    beginn: prozessabhängig
    hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; Frist und Beginn
      fachlich zu validieren.
letzte-aktualisierung: '2026-08-12'
tags:
- Verlust
- Ausweis
- Meldung
---



# Verlustanzeige Ausweisdokument

## Definition

Daten zur Anzeige des Verlusts eines Identitätsdokuments gegenüber Behörden.

## Felder

- Dokumentart
- Dokumentnummer
- Verlustdatum
- Verlustort
- betroffene Person
- Meldedatum

## Klassifizierung

- Schutzstufe: C
- Schutzbedarf: hoch
- Vertraulichkeit: vertraulich
- BPMN-Typ: nachricht

## Rechtsgrundlagen

- PAuswG
- PassG

## Aufbewahrung

- Frist: prozessabhängig
- Beginn: prozessabhängig
- Hinweis: Aus kommunalen Serviceportaltexten abgeleiteter Datentyp; fachlich zu validieren.

## Verwendung in Prozessen

- Verlust des eigenen Personalausweises melden

*(In KOOS sollte dieser Abschnitt perspektivisch durch Resolver-Rückverweise aus `prozesse/*.md` berechnet werden.)*

## Hinweise

Abgeleiteter Datentyp aus kommunalen Serviceportal-Texten in Niedersachsen; keine offizielle FIM/XDatenfelder-Originaldatei.

KOOS-konforme Konvertierung aus einer älteren Markdown-Sammlung.

Zuständige OE, Klassifizierung und BPMN-Typ sind heuristisch vorbelegt und sollten fachlich überprüft werden.

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

## Schutzstufe geprüft 2026-08-12

**Bleibt bei C.** Dokumentart, Dokumentnummer, Verlustdatum, Verlustort, betroffene Person,
Meldedatum.

**Ausweisdaten ermöglichen Identitätsmissbrauch**, und der trifft die wirtschaftlichen
Verhältnisse — das Kriterium der Stufe C. `dstore-ausweisdokument` steht bereits geprüft auf C.

**Nicht D.** Identitätsmissbrauch bedroht nicht die Existenz im Sinne des LfD-Konzepts, das
dort Gesundheitsdaten, Sozialdaten, Schulden und Straffälligkeit nennt.

**Zum Zeitfenster:** Die Verlustanzeige entsteht genau in der Phase, in der das Dokument noch
missbraucht werden kann — zwischen Verlust und Sperrung. Die Dokumentnummer ist in dieser
Phase das missbrauchsrelevante Datum.

*Durchsicht Los 2 (Amt 33) vom 2026-08-12. Grundlage: `_output/vvt-datenspeicher-laeufe/VORSCHLAG-2026-08-12-los2-amt33.md`.*
