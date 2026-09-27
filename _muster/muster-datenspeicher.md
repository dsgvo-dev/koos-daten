---
# Muster Datenspeicher. Datei kopieren nach daten/dstore-<kurzname>.md und alle <Platzhalter> ersetzen.
# Kommentarzeilen (#) vor dem Speichern entfernen. Wertelisten: koos.yaml, Abschnitt vokabular.
id: dstore-<kurzname>
# Stabile ID = Dateiname ohne .md. Niemals nachträglich ändern.
typ: datenspeicher
system: null
# Konkretes IT-Verfahren nur, wenn es für die Einordnung nötig ist; sonst null. Keine Herstellernamen.
name: <Anzeigename, z. B. Schlüsselverwaltung>
zuständige-einheit: oe-<id>
bpmn:
  typ: datenobjekt
  # datenobjekt (Vorgangsdaten) | datenspeicher (dauerhafter Bestand) | nachricht (Übermittlung)
# personenbezug: nein
# Nur setzen, wenn der Datensatz keiner natürlichen Person zuzuordnen ist. Dann bleibt schutzstufe leer.
klassifizierung:
  # Datenschutz -- Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: <A|B|C|D|E>
  # Im Zweifel die höhere Stufe. Begründung im Abschnitt Hinweise.
  schutzbedarf: <normal|hoch>
  # Ergebnis nach der Datenschutz-Vorgehensweise (Maximum aller Achsen), zweiwertig.
  vertraulichkeitsklasse: <öffentlich|intern|vertraulich|streng vertraulich>
  # Eigenständige Achse (ISO/IEC 27002, 5.12), nicht aus der Schutzstufe ableiten.
  # Informationssicherheit -- Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: <normal|hoch|sehr hoch>
  bsi-integritaet: <normal|hoch|sehr hoch>
  bsi-verfuegbarkeit: <normal|hoch|sehr hoch>
  bsi-schutzbedarf: <Maximum der drei BSI-Werte>
  rechtsgrundlagen:
  - gesetz: <Kurzbezeichnung, z. B. DSGVO>
    artikel: <z. B. Art. 6 Abs. 1 lit. e>
  aufbewahrung:
    frist: <z. B. 3 Jahre>
    beginn: <z. B. nach Abschluss des Vorgangs>
    hinweis: <Rechtsgrundlage der Frist, z. B. Aktenplan, § 147 AO>
letzte-aktualisierung: '<JJJJ-MM-TT>'
tags:
- <Schlagwort>
# Nur für Kontextvarianten nach regeln/kontextregeln.yaml: Block kontext (rolle, variante-von, bedingung, stufe-basis, stufe-variante, regelquelle).
---

# <Anzeigename>

## Definition

<Was ist dieser Datenspeicher, welche Vorgänge dokumentiert er, was dokumentiert er ausdrücklich nicht.>

## Felder

- <Datenfeld>
- <Datenfeld>

## Hinweise

**Schutzstufe <X>.** <Begründung anhand des Schutzstufenkonzepts: warum nicht die nächstniedrigere, warum nicht die nächsthöhere.>

**Art. 9/10-Daten.** <Enthalten oder nicht enthalten, mit Begründung.>

**BSI-Schutzziele.** <Begründung für Integrität und Verfügbarkeit, soweit abweichend von normal.>
