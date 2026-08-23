---
id: dstore-bauakte
typ: datenspeicher
system: null
name: Bauakte
zuständige-einheit: oe-amt-63
bpmn:
  typ: datenspeicher
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
  - gesetz: NBauO
    artikel: §88
    titel: Aufbewahrungspflichten der Bauaufsichtsbehörde
  - gesetz: NArchG
    titel: Niedersächsisches Archivgesetz
  aufbewahrung:
    frist: dauerhaft (Archiv) oder 30 Jahre nach Abschluss des letzten Verfahrens
    beginn: nach Abschluss des jeweiligen Verfahrens
    hinweis: Akteneinsicht nach §1 NArchG und auf Antrag (proc-bauaktenarchiv-akteneinsicht-bereitstellung,
      proc-bauaktenarchiv-akteneinsicht-beantragen)
letzte-aktualisierung: '2026-08-10'
---


# Bauakte

## Definition

Gesamtheit aller Unterlagen, die zu einem Bauvorhaben auf einem Grundstück entstanden sind.
Die Bauakte ist der persistente Datenspeicher des Bauamts: Sie besteht unabhängig von
einzelnen Prozessinstanzen, wird über Jahrzehnte geführt und ist Grundlage für spätere
Verfahren, Akteneinsichten und Behördenabfragen.

Im BPMN-Sinne ist die Bauakte ein **Data Store** — kein Datenobjekt, das einen Prozess
durchläuft, sondern ein dauerhafter Speicher, aus dem Prozesse lesen und in den sie schreiben.

## Typische Inhalte

- Alle Bauanträge, Bauvoranfragen und Bauvorbescheide zum Grundstück
- Erteilte Baugenehmigungen (mit gestempelten Bauzeichnungen)
- Fachstellungnahmen und interne Vermerke
- Ablehnungsbescheide und Widerspruchsentscheidungen
- Abbruchanzeigen und Nutzungsänderungen

## Hinweise

Akteneinsicht ist auf Antrag möglich (proc-bauaktenarchiv-akteneinsicht-bereitstellung / proc-bauaktenarchiv-akteneinsicht-beantragen). Einsichtsberechtigt
sind in der Regel Eigentümer/innen des Grundstücks, Rechtsnachfolger/innen sowie Personen
mit berechtigtem Interesse. Die Bauakte kann auch als Grundlage für Auskunftsersuchen
anderer Behörden dienen.

## BSI-Vektoren geprüft 2026-08-04

**Integrität hoch.** Auf die Richtigkeit dieses Datenbestands verlassen sich andere -- Behörden, Gerichte oder die betroffene Person selbst. Eine unbemerkte Verfälschung führt nicht zu einem Fehler im Einzelfall, sondern zu falschen Folgeentscheidungen, die auf dem Bestand aufbauen.

Die Bauakte ist über die gesamte Lebensdauer eines Gebäudes der Nachweis für Bestandsschutz und Genehmigungslage.

## Schutzstufe geprüft 2026-08-10

**B → D.** **Die Bauakte ist ein Trägerobjekt, kein eigenständiger Inhalt.** Sie besteht nach § 4 NBauO grundstücksbezogen und nimmt alles auf, was im Verfahren anfällt. Nach dem Maximalprinzip richtet sich ihre Stufe deshalb nach dem sensibelsten Bestandteil.

Das ist die **Nachbareinwendung** -- am selben Tag auf Stufe D eingestuft, weil § 68 Abs. 2 NBauO ein Beteiligungsrecht mit unbegrenztem Freitext gewährt. Hinzu kommen Anträge auf barrierefreies Bauen oder auf einen Umbau wegen Pflegebedürftigkeit; sie lassen eine Behinderung erkennen und fallen unter Art. 9 DSGVO.

**Praktische Folge:** Bei der Akteneinsicht Dritter nach § 29 VwVfG darf nicht die Akte als Ganzes herausgegeben werden. Es ist Bestandteil für Bestandteil zu prüfen, was dem Einsichtsrecht unterliegt.
