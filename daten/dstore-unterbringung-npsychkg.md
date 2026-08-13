---
id: dstore-unterbringung-npsychkg
typ: datenspeicher
system: null
name: Unterbringungsverfahren nach NPsychKG
datenkategorie: Gesundheit & Soziales
zuständige-einheit: oe-amt-54
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
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c, lit. d, lit. e
  - gesetz: DSGVO
    artikel: Art. 9 Abs. 2 lit. b, lit. g, lit. i
  - gesetz: NPsychKG
    artikel: § 33 (besonders schutzwürdige Daten — bereichsspezifische Erlaubnis für
      Daten nach Art. 9 Abs. 1 DSGVO und berufs- oder amtsgeheimnisgeschützte Daten)
  - gesetz: NPsychKG
    artikel: § 16 (sofortige Unterbringung), §§ 17-29 (Unterbringung durch Verwaltungsbehörde,
      gerichtliches Verfahren)
  - gesetz: FamFG
    artikel: §§ 312 ff. (Verfahren in Unterbringungssachen)
  aufbewahrung:
    frist: 10 Jahre
    beginn: nach Abschluss des Unterbringungsverfahrens
letzte-aktualisierung: '2026-08-10'
tags:
- Unterbringung
- Zwangsmaßnahme
- Freiheitsentziehung
- NPsychKG
---



# Unterbringungsverfahren nach NPsychKG

## Definition

Dokumentation eines behördlichen Unterbringungsverfahrens für psychisch Kranke nach dem NPsychKG — von der Gefährdungseinschätzung über die Anordnung bis zur Beendigung der Unterbringung. Kern des Verfahrens ist die Freiheitsentziehung einer natürlichen Person zum Schutz von Leben und Gesundheit (Eigen- oder Fremdgefährdung).

## Felder

- betroffene Person (Name, Geburtsdatum)
- Diagnose und Gefährdungseinschätzung
- Einweisungsgründe (konkrete Gefährdungslage, akute Selbst-/Fremdgefährdung)
- Art der Unterbringung (sofortig nach § 16 NPsychKG oder nach gerichtlicher Entscheidung)
- unterbringende Einrichtung (Klinik)
- beteiligte Angehörige und Kontaktpersonen
- gerichtliche Entscheidungen nach FamFG §§ 312 ff.
- Verfahrensstand und Rechtskraftvermerk

## Hinweise

**Angelegt am 2026-08-04, Anlass: vvt-54-001, Durchgang 01.**

- **Abgrenzung zu dstore-gesundheitsdaten (D):** Gesundheitsdaten trägt Diagnose, Therapie und medizinische Befunde. Dieser Speicher trägt die *freiheitsentziehende Maßnahme selbst* — die Information, dass eine Person gegen oder ohne ihren Willen in einer geschlossenen Einrichtung untergebracht ist oder war. Nicht die Diagnose ist das höchste Schutzgut, sondern die Tatsache der Freiheitsentziehung.
- **Stufe E:** Nach dem Schutzstufenkonzept des LfD Niedersachsen erfasst E den Missbrauch, der „Gesundheit, Leben oder Freiheit" beeinträchtigt. Eine Unterbringung nach NPsychKG ist eine solche Beeinträchtigung der Freiheit — sie trifft zu, unabhängig von der konkreten Diagnose. Das Maximalprinzip (R6) gebietet die Stufe nach der sensibelsten Angabe, die anfallen kann; bei einer sofortigen Unterbringung nach § 16 NPsychKG ist das der Entzug der Freiheit selbst.
- **Vier weitere Einträge tragen Stufe E:** `dstore-anmeldebescheinigung-prostschg`, `dstore-hiv-beratung-pseudonym`, `dstore-auskunftssperre-melderegister` und `dstore-einsatzdokumentation-notruf`. Dieser Speicher ist der fünfte.
- **Kein allgemeiner Gesundheitsspeicher:** `dstore-gesundheitsdaten` ist ein übergreifender Speicher, der an vielen Verarbeitungstätigkeiten hängt (Art. 9, Schutzstufe D). Eine Anhebung auf E ist dort nicht gerechtfertigt und würde auf alle Gesundheitsdaten der Kommune durchschlagen. Die Freiheitsentziehung rechtfertigt eine eigene Stufe, aber nur für die Verarbeitungstätigkeiten, die tatsächlich eine Unterbringung dokumentieren.

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
