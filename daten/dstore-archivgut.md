---
id: dstore-archivgut
typ: datenspeicher
system: null
name: Archivgut
zuständige-einheit: oe-amt-41
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
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. e
  - gesetz: NDSG
    artikel: § 3
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. j
    titel: Öffnungsklausel für Archivzwecke im öffentlichen Interesse; die Erlaubnis
      selbst folgt aus § 3b NArchG
  - gesetz: NArchG
    artikel: § 3b
    titel: Verarbeitung besonderer Kategorien personenbezogener Daten ist zulässig;
      sie berührt stets schutzwürdige Interessen der betroffenen Person
  - gesetz: NArchG
    artikel: § 7 Abs. 3 Satz 2
    titel: Geltung der §§ 3a, 3b, 4 Satz 1 und 5 bis 6a für kommunale Archive
  - gesetz: NArchG
    artikel: § 4 Satz 1
    titel: dauerhafte und sichere Verwahrung
  - gesetz: NArchG
    artikel: § 5
    titel: Nutzung des Archivgutes, Schutzfristen
  - gesetz: NArchG
    artikel: § 6a
    titel: Ausschluss der Rechte aus Art. 16 Satz 1, 18, 20 und 21 DSGVO für Archivgut
  aufbewahrung:
    frist: dauerhaft
    beginn: mit Übernahme in das Archiv
    hinweis: >-
      Archivgut wird nicht geloescht, sondern nach § 4 Satz 1 NArchG auf Dauer und
      sicher verwahrt. Fuer die Nutzung gelten die Schutzfristen des § 5 Abs. 2 NArchG:
      30 Jahre nach der letzten inhaltlichen Bearbeitung, 50 Jahre bei besonders
      geheimhaltungsbeduerftigem Schriftgut, bei personenbezogenem Archivgut fruehestens
      10 Jahre nach dem Tod der betroffenen Person oder, wenn das Sterbedatum nicht
      feststellbar ist, 100 Jahre nach ihrer Geburt.
letzte-aktualisierung: '2026-08-15'
tags:
- Archivgut
- Kommunalarchiv
- Schutzfrist
- besondere Kategorien
- historisches Schriftgut
---

# Archivgut

## Definition

Schriftgut von bleibendem Wert, das das Kommunalarchiv nach § 2 Abs. 2 NArchG übernommen hat
und dauerhaft verwahrt. Schriftgut umfasst nach § 2 Abs. 1 NArchG nicht nur Akten und
Urkunden, sondern auch Karten, Pläne, Bild-, Film- und Tonaufzeichnungen, Karteien und
Dateien.

Die Datenart betrifft **nicht** die Antragstellenden einer Recherche — deren Daten führt
`dstore-personenstammdaten` —, sondern die **im Archivgut selbst enthaltenen
personenbezogenen Daten Dritter**.

## Felder

- Bestands- und Signaturangaben
- Laufzeit des Vorgangs
- im Schriftgut enthaltene personenbezogene Daten Dritter, je nach Bestand
- ggf. besondere Kategorien nach Art. 9 Abs. 1 DSGVO in historischem Schriftgut
- Angaben zur Schutzfrist und zu ihrem Ablauf
- Vermerke zur Nutzung und zu erteilten Verkürzungen

## Abgrenzung

| | |
|---|---|
| `dstore-personenstammdaten` | Daten der Antragstellenden: Name, Anschrift, Kontakt, Forschungszweck |
| **`dstore-archivgut`** | Daten der Personen, über die das Archivgut Auskunft gibt |
| `dstore-verwaltungsakte` | laufendes Verwaltungsschriftgut, noch nicht archiviert |

## Schutzstufe geprüft 2026-08-15

**Stufe D.** Die Einstufung folgt nicht aus einer Einschätzung, sondern aus einer
gesetzlichen Wertung. **§ 3b Satz 2 NArchG** im Wortlaut:

> Die Verarbeitung besonderer Kategorien personenbezogener Daten im Sinne des Artikels 9
> Abs. 1 der Datenschutz-Grundverordnung ist zulässig. **Sie berührt stets schutzwürdige
> Interessen der betroffenen Person im Sinne des § 5 Abs. 2 Satz 5.**

Das LfD-Schutzstufenkonzept ordnet besondere Kategorien nach Art. 9 DSGVO der Stufe D zu.

**Warum nicht C.** Archivgut ist kein Verwaltungsschriftgut im laufenden Betrieb. Es kann
Fürsorge-, Gesundheits-, Entnazifizierungs- und Personenstandsunterlagen enthalten — genau
die Kategorien, für die § 3b geschaffen wurde.

**Warum nicht E.** Stufe E setzt Gefahr für Leib, Leben oder persönliche Freiheit voraus. Die
Schutzfristen des § 5 Abs. 2 NArchG — frühestens zehn Jahre nach dem Tod der betroffenen
Person — schließen den akuten Gefährdungsfall im Regelbetrieb aus. Ergibt sich im Einzelfall
eine Gefährdungslage, greift der Kontextanheber `dstore-schutzbeduerftigkeitskennzeichen`
aus `regeln/kontextregeln.yaml`.

**Zur Rechtsgrundlage.** Art. 9 Abs. 2 lit. j DSGVO ist keine Erlaubnisnorm, sondern eine
Öffnungsklausel — sie erlaubt die Verarbeitung nur „auf der Grundlage des Unionsrechts oder
des Rechts eines Mitgliedstaats". Die Erlaubnis ist **§ 3b NArchG**. Für ein kommunales
Archiv tritt **§ 7 Abs. 3 Satz 2 NArchG** hinzu, weil § 3b unmittelbar nur für das
Landesarchiv gilt. Die Kette lautet vollständig:
`Art. 9 Abs. 2 lit. j DSGVO i. V. m. § 3b NArchG i. V. m. § 7 Abs. 3 Satz 2 NArchG`.

Normen geprüft am 2026-08-15 an `facts/gesetze/land/narchg.md` und an NI-VORIS. §§ 3b und 7
stehen dort jeweils in der Fassung ab 25.05.2018 und sind zeichengleich mit dem Bestandstext.
**Hinweis:** Der Gesamtvermerk unserer Fundstelle („zuletzt geändert 16.05.2018") ist
überholt; geltend ist Artikel 3 des Gesetzes vom 27.03.2025. Die hier tragenden Paragraphen
sind davon nicht betroffen. Der Befund ist im Tagesprotokoll vom 2026-08-15 vermerkt.

## BSI-Vektoren geprüft 2026-08-15

**Integrität: `hoch`.** § 4 Satz 1 NArchG verlangt, Archivgut „zu erhalten und vor unbefugter
Nutzung, vor Beschädigung oder Vernichtung zu schützen". Eine Verfälschung ist irreversibel —
Archivgut ist Unikat, es gibt keine Zweitüberlieferung, aus der sich der richtige Stand
wiederherstellen ließe.

**Verfügbarkeit: `normal`**, geprüft an der Frage des Durchgangs vom 2026-08-04:
*Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* — Nein. Ein Ausfall
verzögert eine Recherche, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Vertraulichkeit: `hoch`.** Die Offenlegung von Archivgut vor Ablauf der Schutzfrist träfe
die Kommune als verantwortliche Stelle unmittelbar; § 5 Abs. 2 NArchG ist eine gesetzliche
Nutzungssperre, kein Ermessen.

## Besonderheit: eingeschränkte Betroffenenrechte

Für Archivgut bestehen nach **§ 6a NArchG** die Rechte aus Art. 16 Satz 1 (Berichtigung),
Art. 18 (Einschränkung), Art. 20 (Datenübertragbarkeit) und Art. 21 (Widerspruch) DSGVO sowie
die Mitteilungspflicht nach Art. 19 DSGVO **nicht**. An ihre Stelle tritt § 6 NArchG — Recht
auf Auskunft und Gegendarstellung.

Das ist bei der Ableitung technischer und organisatorischer Maßnahmen zu berücksichtigen:
Maßnahmen, die allein der Umsetzung dieser Rechte dienen, laufen hier leer.

## Hinweise

Angelegt am 2026-08-15 aufgrund eines Befundes der Bestandsprüfung: `vvt-41-003`
(Kommunalarchiv — Nutzung und Recherche) beruft sich in der Rechtsgrundlage auf Art. 9
Abs. 2 lit. j DSGVO und benennt in `kategorien_betroffener` und `kategorien_daten`
ausdrücklich die Drittbetroffenen und die besonderen Kategorien im historischen Schriftgut,
führte aber allein `dstore-personenstammdaten` der Stufe C. Der Befund wurde erst sichtbar,
nachdem `pruefung.py` am 2026-08-15 auf alle aktiven VVT umgestellt wurde.

Vorschlag und Belege: `_output/VORSCHLAG-2026-08-15-archivgut-vvt-41-003.md`.
