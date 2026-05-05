---
id: dstore-bauakte
typ: datenspeicher
system: null
name: Bauakte
datenkategorie: Bescheid / Nachweis
zuständige-einheit: oe-amt-63
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: B
  schutzbedarf: hoch
  vertraulichkeit: intern
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
letzte-aktualisierung: 2026-04-07
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
