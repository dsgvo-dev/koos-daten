---
id: dstore-einsatzdokumentation-notruf
typ: datenspeicher
system: null
name: Notruf und Einsatzdokumentation
datenkategorie: Feuerwehr & Brandschutz
zuständige-einheit: oe-amt-37
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: E
  schutzbedarf: hoch
  vertraulichkeitsklasse: streng vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: sehr hoch
  bsi-integritaet: hoch
  bsi-verfuegbarkeit: hoch
  bsi-schutzbedarf: sehr hoch
  rechtsgrundlagen:
  - gesetz: NRettDG
    artikel: § 11 Abs. 1
    titel: Aufzeichnungspflicht der Rettungsleitstelle
  - gesetz: NRettDG
    artikel: § 11 Abs. 2
    titel: Zulässige Verarbeitungszwecke
  - gesetz: NRettDG
    artikel: § 11 Abs. 4
    titel: Verarbeitung besonderer Kategorien nach Art. 9 Abs. 1 DSGVO
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. g
  - gesetz: NBrandSchG
    artikel: §§ 35a ff.
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Abschluss des Einsatzes
    hinweis: Einsatzdokumentation als Nachweis gegenüber Aufsicht, Versicherungen
      und Gerichten; § 197 BGB bei geltend gemachten Ansprüchen.
letzte-aktualisierung: '2026-08-10'
tags:
- Feuerwehr
- Rettungsdienst
- Notruf
- Schutzstufe E
---



# Notruf und Einsatzdokumentation

## Definition

Aufnahme eines Hilfeersuchens und Dokumentation des daraufhin geführten Einsatzes von Feuerwehr und Rettungsdienst.

## Felder

- Notrufabsetzende Person mit Rufnummer
- Standort und Meldebild
- Einsatzort und Einsatzzeit
- Art des Einsatzes
- betroffene Personen (Verletzte, Geschädigte, Vermisste)
- Gesundheitsdaten bei Personenschäden
- eingesetzte Kräfte und Fahrzeuge
- Einsatzverlauf und Einsatzergebnis
- Übergabe an Polizei oder Klinik

## Hinweise

Angelegt am 2026-08-03 zu `vvt-37-001` (Hilfeersuchen, Einsatzdokumentation und
Aufgabenwahrnehmung Feuerwehr).

**Die Rechtsgrundlage ist § 11 NRettDG -- eine bereichsspezifische Datenschutznorm.**
Absatz 1 verpflichtet die Rettungsleitstelle, die einsatzbedingte Telekommunikation
aufzuzeichnen und über jeden Einsatz ein Protokoll zu fertigen; die Träger stellen sicher,
dass über jede Fahrt eines Rettungsmittels und jeden Notarzteinsatz ein Bericht und über
jede Patientenübergabe ein Protokoll gefertigt wird.

**Absatz 4 erlaubt ausdrücklich die Verarbeitung besonderer Kategorien** nach Art. 9 Abs. 1
DSGVO. Damit ist die Erlaubnisnorm für die Gesundheitsdaten benannt und muss nicht über
Art. 9 Abs. 2 lit. c) konstruiert werden.

**Absatz 2 Satz 2 zählt die zulässigen Zwecke abschließend auf:**

1. medizinische Betreuung der behandelten oder beförderten Person
2. Abrechnung der erbrachten Leistungen
3. Vorbereitung oder Durchführung gerichtlicher Verfahren und Verwaltungsverfahren
4. Qualitätsmanagement
5. Aus-, Fort- und Weiterbildung des eingesetzten Personals
6. Ermittlung des Bedarfs an Rettungsmitteln

Jede andere Verwendung bedarf der Einwilligung der betroffenen Person.

**Für die Zwecke 4 bis 6 sind die Daten zu anonymisieren, soweit der Verwendungszweck es
zulässt** (§ 11 Abs. 2 Satz 3 NRettDG). Qualitätsmanagement, Ausbildung und Bedarfsplanung
dürfen also nicht mit personenbezogenen Einsatzprotokollen betrieben werden, wenn
anonymisierte Auswertungen genügen. Das ist keine Empfehlung, sondern Gesetzesbefehl und
gehört in die Zugriffsregelung.

**Übermittlung an die Polizei nur im gesetzlich benannten Umfang.** § 11 Abs. 3 NRettDG
erlaubt die Übermittlung von Name, Geburtsdatum, Anschrift, Verbleib und
Staatsangehörigkeit an die Polizeidirektion Hannover -- und zwar allein zum Zweck der
Vermisstensuche und der Familienzusammenführung. Weitere Angaben und weitere Zwecke deckt
die Norm nicht.

**Stufe E nach dem Maximalprinzip.** Die Einsatzdokumentation kann alles enthalten, was
einen Notruf auslöst: eine Überdosis, einen Suizidversuch, häusliche Gewalt, einen
Brandstiftungsverdacht. Wird bekannt, dass unter einer Anschrift ein Notruf abgesetzt wurde
und weshalb, kann das die betroffene Person unmittelbar gefährden.

**Die notrufabsetzende Person ist eine eigene Betroffene.** Sie ist oft nicht die
geschädigte Person, sondern Nachbarin, Passant oder Angehöriger. Ihre Rufnummer wird
technisch übermittelt, ohne dass sie darüber entscheidet.

## BSI-Vektoren geprüft 2026-08-04

**Integrität: `hoch`** · **Verfügbarkeit: `hoch`**

**Über `normal` gesetzt: Integrität `hoch` und Verfügbarkeit `hoch`.** Die Festlegung stammt aus dem BSI-Durchgang vom 2026-08-04, in dem 67 Speicher angehoben wurden. Die Begründung erfolgte gruppenweise; die sechs Gruppen — Register und Urkunden, Entscheidungsgrundlagen, Gefahrenabwehr für die Integrität sowie breite Nutzung, gesetzliche Fristen, Gefahrenabwehr und Veterinärwesen für die Verfügbarkeit — sind in `skills/vvt-datenspeicher/SKILL.md`, Abschnitt 10, benannt.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Text berichtigt am 2026-08-12.* An dieser Stelle stand der Sammelvermerk
„Integrität und Verfügbarkeit bleiben bei `normal`" samt drei verneinten Prüffragen. Das
widersprach den Werten im Frontmatter dieser Datei. Der Baustein war am 2026-08-04 flächig
eingesetzt worden, ohne ihn an die tatsächlichen Werte anzupassen — in 105 Dateien.
**Die Werte selbst wurden nicht geändert**; maßgeblich ist das Frontmatter, und die
Kettenprüfung E3 rechnet mit ihm.

## Schutzstufe geprüft 2026-08-10

**Bleibt bei E.** Die Einstufung wurde am 2026-08-04 bei der Anlage beziehungsweise
Überarbeitung dieses Speichers ausführlich begründet -- siehe die Hinweise oben. Der
Durchgang vom 2026-08-10 hat sie bestätigt und trägt hier nur den Prüfvermerk nach, der bisher
fehlte.

*Der Vermerk ist kein Formalismus: Ohne ihn zählte der Speicher als ungeprüft, und der
Rückstand wies 129 statt der tatsächlich offenen 115 Speicher aus -- allesamt auf Stufe C.*
