---
id: dstore-waffenrechtliche-erlaubnis
typ: datenspeicher
system: null
name: Waffenrechtliche Erlaubnis und Jagdschein
datenkategorie: Ordnung & Erlaubnisse
zuständige-einheit: oe-amt-32
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
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c
  - gesetz: DSGVO
    artikel: Art. 10
  - gesetz: WaffG
    artikel: §§ 4, 10, 26
  - gesetz: BJagdG
    artikel: § 15
  - gesetz: SprengG
    artikel: § 7
  aufbewahrung:
    frist: 3 Jahre nach Erlöschen aller Erlaubnisse
    beginn: mit dem Erlöschen der letzten Erlaubnis
    hinweis: § 26 WaffG für das Nationale Waffenregister; Jagdscheindaten 10 Jahre
      entsprechend kommunaler Aktenordnung.
letzte-aktualisierung: '2026-08-10'
tags:
- Waffenrecht
- Jagdrecht
- Art. 10 DSGVO
---



# Waffenrechtliche Erlaubnis und Jagdschein

## Definition

Erteilte Erlaubnisse nach Waffen-, Jagd- und Sprengstoffrecht einschließlich der eingetragenen Waffen und der Nachweise über die Aufbewahrung.

## Felder

- Erlaubnisinhaberin oder -inhaber
- Art und Nummer der Erlaubnis (Waffenbesitzkarte, Jagdschein, Sprengstofferlaubnis)
- eingetragene Waffen mit Kennzeichen
- Bedürfnisgrund
- Sachkundenachweis
- Nachweis der sicheren Aufbewahrung nach § 36 WaffG
- Ergebnisse der Aufbewahrungskontrolle
- Gültigkeit und Erlöschen

## Hinweise

Angelegt am 2026-08-03 zu `vvt-32-017` (Waffen-, Jagd- und Sprengstoffwesen).

**Stufe D nach dem Maximalprinzip.** Die Erlaubnis setzt eine Zuverlässigkeitsprüfung nach § 5 WaffG voraus, die auf Auskünfte aus dem Bundeszentralregister und dem staatsanwaltschaftlichen Verfahrensregister zugreift. Zusammen mit der Angabe, welche Waffen eine Person besitzt und wo sie sie verwahrt, ergibt das eine Information, deren Offenbarung erhebliche Folgen haben kann -- bis hin zur Gefährdung durch Dritte, die sich Zugang verschaffen wollen.

**Der Bedürfnisgrund verrät die Vereinszugehörigkeit.** Bei Sportschützen ergibt sich das Bedürfnis aus der Mitgliedschaft in einem schießsportlichen Verein, bei Jägern aus dem Jagdschein. Das ist keine besondere Kategorie nach Art. 9, aber eine Angabe, die für sich genommen Rückschlüsse zulässt.

VERWORFEN bei der Zuordnung: `dstore-fischereischein-sachkunde` -- Fischereirecht, nicht Jagdrecht; der Speicher war über die gemeinsame „Sachkunde" vorgeschlagen worden.

## BSI-Vektoren geprüft 2026-08-04

**Verfügbarkeit hoch.** Der Bestand wird in einer Gefahrenlage gebraucht, in der es auf Minuten ankommt. Ein Ausfall bedeutet, dass die Kommune die Lage nicht einschätzen kann.

Bei einer Kontrolle oder einem Vorfall muss binnen Minuten feststellbar sein, wer welche Waffen besitzt und wo sie verwahrt werden.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei D.** Die Einstufung wurde am 2026-08-04 bei der Anlage beziehungsweise
Überarbeitung dieses Speichers ausführlich begründet -- siehe die Hinweise oben. Der
Durchgang vom 2026-08-10 hat sie bestätigt und trägt hier nur den Prüfvermerk nach, der bisher
fehlte.

*Der Vermerk ist kein Formalismus: Ohne ihn zählte der Speicher als ungeprüft, und der
Rückstand wies 129 statt der tatsächlich offenen 115 Speicher aus -- allesamt auf Stufe C.*
