---
id: dstore-bauantrag
typ: datenspeicher
system: null
name: Bauantrag
zuständige-einheit: oe-amt-63
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: NBauO
    artikel: §63
    titel: Baugenehmigungsverfahren
  - gesetz: NBauO
    artikel: §64
    titel: Vereinfachtes Genehmigungsverfahren
  - gesetz: VwVfG
    artikel: §22
    titel: Einleitung des Verfahrens
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c
    titel: gesetzliche Verpflichtung
  aufbewahrung:
    frist: 10 Jahre nach Abschluss des Verfahrens
    beginn: nach Bestandskraft des Bescheids oder Ablehnung
    hinweis: Bestandteil der Bauakte; Aufbewahrungsfrist kann je nach Gemeinde abweichen
letzte-aktualisierung: '2026-08-10'
---


# Bauantrag

## Definition

Formeller Antrag einer Bauherrin oder eines Bauherrn an die Bauaufsichtsbehörde zur Erteilung
einer Baugenehmigung. Der Bauantrag löst das Baugenehmigungsverfahren aus und bildet zusammen
mit den Antragsunterlagen das Kerndokument der Bauakte.

## Typische Inhalte

- Angaben zur Bauherrin / zum Bauherrn und zur Entwurfsverfasserin / zum Entwurfsverfasser
- Beschreibung des Bauvorhabens (Art, Umfang, Nutzung)
- Grundstücksangaben (Flurstücknummer, Gemarkung)
- Verzeichnis der beigefügten Antragsunterlagen
- Unterschriften Bauherr/in und Entwurfsverfasser/in

## Hinweise

Der Bauantrag ist zwingend durch eine bauvorlagenberechtigte Person (z.B. Architekt/in)
zu unterschreiben (§ 53 NBauO). Unvollständige Anträge werden mit Nachforderungsschreiben
zurückgegeben; die Frist zur Entscheidung beginnt erst mit vollständigen Unterlagen.

## BSI-Vektoren geprüft 2026-08-04

**Integrität bleibt normal.** Der Bestand ist ein **vorgelegter Nachweis**, keine Registerführung. Die Kommune prüft ihn im Verfahren und trifft auf seiner Grundlage eine Entscheidung; sie führt ihn aber nicht als Bestand, auf dessen Richtigkeit sich Dritte dauerhaft verlassen.

Der Unterschied ist wesentlich: Wird ein Melderegister unbemerkt verfälscht, sind alle Folgeauskünfte falsch. Wird eine vorgelegte Verdienstbescheinigung verfälscht, wirkt sich das auf das eine Verfahren aus, in dem sie vorgelegt wurde -- und die ausstellende Stelle kann sie erneut ausstellen.

**Verfügbarkeit bleibt unverändert.** Der Nachweis kann bei Verlust nachgefordert werden; ein Ausfall verzögert das Verfahren, verhindert es aber nicht.

Geprüft im Durchgang „Register und Nachweise" vom 2026-08-04, in dem 38 Speicher mit Registercharakter, Rechtswirkung oder Gefahrenabwehrbezug auf hohe Integrität angehoben wurden. Dieser gehört nicht dazu.

## Schutzstufe geprüft 2026-08-10

**B → C.** Die Bau-Grunddaten sind mehr als Sachdaten.

Der Antrag führt Bauherrschaft, Vorhaben und Grundstück zusammen und nimmt die Begründung des Vorhabens auf. Bei Anträgen für Anbauten zur Pflege von Angehörigen oder für barrierefreie Umbauten wird der Anlass mitgeteilt.

**Kohärenz:** `dstore-bauakte` steht seit dem 2026-08-10 auf Stufe D, weil sie die Nachbareinwendung aufnimmt. Die Einzelbestandteile tragen diese Stufe nicht -- sie tragen aber auch nicht mehr die Stufe B, die sie aus dem Import mitgebracht hatten.
