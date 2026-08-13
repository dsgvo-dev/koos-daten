---
id: dstore-gerichtsverfahren
typ: datenspeicher
system: null
name: Gerichtsverfahren
datenkategorie: Recht & Compliance
zuständige-einheit: oe-amt-30
bpmn:
  typ: datenobjekt
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
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. e
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. f
  - gesetz: DSGVO
    artikel: Art. 10
  - gesetz: NDSG
    artikel: § 3
  - gesetz: NKomVG
    artikel: § 86 Abs. 1 Satz 2
  - gesetz: BGB
    artikel: §§ 195, 197 Abs. 1 Nr. 3
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach rechtskräftigem Abschluss des Verfahrens
    hinweis: Festlegung des Trägers. Ist ein Anspruch rechtskräftig festgestellt worden
      -- durch Urteil, Vergleich oder vollstreckbare Urkunde --, beträgt die Aufbewahrung
      30 Jahre nach § 197 Abs. 1 Nr. 3 BGB, weil der Titel so lange vollstreckbar
      bleibt.
letzte-aktualisierung: '2026-08-10'
tags:
- Gerichtsverfahren
- Prozessvertretung
- Rechtsamt
---



# Gerichtsverfahren

## Definition

Verfahrensakte zu gerichtlichen Verfahren, an denen die Kommune beteiligt ist, geführt vom Rechtsamt im Rahmen der Prozessvertretung nach § 86 Abs. 1 Satz 2 NKomVG.

## Felder

- Rechtsweg und zuständiges Gericht
- Aktenzeichen des Gerichts und eigenes Aktenzeichen
- Verfahrensart und Streitgegenstand
- Beteiligte mit ihrer Rolle -- Klagepartei, Beklagte, Beigeladene, Zeuginnen und Zeugen, Sachverständige
- Prozessbevollmächtigte der eigenen und der gegnerischen Seite
- Schriftsätze und gerichtliche Entscheidungen
- Beweismittel, einschließlich der darin enthaltenen besonderen Kategorien personenbezogener Daten
- Verfahrensstand und Termine
- Rechtskraftvermerk und Angabe, ob ein vollstreckbarer Titel vorliegt

## Hinweise

Angelegt am 2026-07-30 zusammen mit `proc-gerichtsverfahren-fuehren` und `vvt-30-004`. `dstore-verwaltungsakte` trägt den Verwaltungsvorgang, nicht die Gerichtsakte; für diese gilt eine andere Frist und ein engerer Zugriff.

**Der Rechtskraftvermerk steuert die Frist.** Ohne die Angabe, ob ein vollstreckbarer Titel vorliegt, lässt sich nicht entscheiden, ob zehn oder dreißig Jahre gelten. Deshalb ist er ein Feld und keine Randnotiz.

**Beweismittel sind der unbestimmteste Teil dieses Speichers.** Was in einem Verfahren vorgelegt wird, bestimmt die Gegenseite mit -- ärztliche Unterlagen im Sozial- oder Amtshaftungsprozess, Ermittlungsakten bei strafrechtlichem Bezug. Deshalb sind Art. 9 Abs. 2 lit. f) und Art. 10 DSGVO von vornherein als Grundlage benannt und nicht erst im Einzelfall nachgetragen.

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

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** **Straffälligkeit, Verdacht und Zuverlässigkeitsprüfung.** Das LfD-Schutzstufenkonzept nennt Straffälligkeit bei Stufe D; Art. 10 DSGVO stellt Daten über strafrechtliche Verurteilungen und Straftaten unter einen eigenen Vorbehalt. Die Einstufung aus dem Import ist zutreffend und wird bestätigt.

**Der Verdacht wiegt hier so schwer wie die Feststellung.** Wird bekannt, dass gegen jemanden ermittelt wird, wirkt das unabhängig vom Ausgang -- die spätere Einstellung erreicht selten dieselben Personen wie der ursprüngliche Vorwurf.

*Sammelvermerk der Durchsicht vom 2026-08-10. In demselben Durchgang wurden 17 Speicher herabgestuft, die die Stufe D nicht trugen; dieser gehört nicht dazu.*
