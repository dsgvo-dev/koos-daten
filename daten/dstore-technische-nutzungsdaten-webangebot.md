---
id: dstore-technische-nutzungsdaten-webangebot
typ: datenspeicher
system: null
name: Technische Nutzungsdaten eines Webangebots
datenkategorie: Digitale Verwaltung
zuständige-einheit: oe-amt-15
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
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. e
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. f
  - gesetz: TDDDG
    artikel: § 25
  - gesetz: NDSG
    artikel: § 3
  aufbewahrung:
    frist: 7 Tage
    beginn: nach der Sitzung
    hinweis: Nur solange, wie es zur Abwehr von Störungen und Angriffen erforderlich
      ist. Längere Vorhaltung bedarf einer eigenen Begründung.
letzte-aktualisierung: '2026-08-04'
tags:
- Webangebot
- IP-Adresse
- TDDDG
---


# Technische Nutzungsdaten eines Webangebots

## Definition

Verbindungs- und Sitzungsdaten, die beim Aufruf eines Webangebots der Kommune technisch anfallen.

## Felder

- IP-Adresse
- Zeitstempel
- Session-ID
- Browsertyp und Betriebssystem
- aufgerufene Funktion
- Fehler- und Störungsmeldungen

## Hinweise

Angelegt am 2026-08-03 zu `vvt-15-002` (Nutzung des Chatbots).

**Die IP-Adresse ist ein personenbezogenes Datum.** Der EuGH hat das für dynamische IP-Adressen entschieden (Urt. v. 19.10.2016, C-582/14 — Breyer), weil der Betreiber rechtliche Mittel hat, die Person über den Zugangsanbieter bestimmen zu lassen.

**§ 25 TDDDG betrifft nicht die Übertragung, sondern die Endeinrichtung.** Für Cookies oder vergleichbare Techniken, die nicht zur Bereitstellung des Dienstes unbedingt erforderlich sind, ist eine Einwilligung nötig. Eine reine Session-ID zur Aufrechterhaltung der Konversation ist erforderlich und einwilligungsfrei; Reichweitenmessung ist es nicht.

Verwendbar für alle Webangebote der Kommune, nicht nur den Chatbot.

## Schutzstufe geprüft 2026-08-14

**C bestätigt.** Verbindungs- und Sitzungsdaten (IP-Adresse, Zeitstempel, Session-ID, Browsertyp). Die IP-Adresse ist personenbezogen (EuGH C-582/14 — Breyer), aber als Logdatum mit 7-Tage-Aufbewahrung ohne Profilbildung. Keine Art. 9-Daten. C ist angemessen.

## BSI-Vektoren geprüft 2026-08-04

**Integrität und Verfügbarkeit bleiben bei `normal`.** Geprüft im Durchgang vom 2026-08-04 anhand von drei Fragen:

1. *Verlassen sich andere dauerhaft auf die Richtigkeit dieses Bestands?* -- Nein. Er wird im Verfahren verwendet und dort geprüft; er ist kein Register, auf das Dritte aufbauen.
2. *Ist er Grundlage einer Entscheidung über einen Menschen, die bei Verfälschung falsch ausfiele?* -- Nicht allein; die Entscheidung stützt sich auf weitere Unterlagen, und eine Abweichung fiele im Verfahren auf.
3. *Knüpft eine Frist oder eine Gefahrenlage an die sofortige Abrufbarkeit?* -- Nein. Ein Ausfall verzögert die Bearbeitung, lässt aber keine Frist verfallen und begründet keine Gefahr.

**Die Vertraulichkeit richtet sich nach der Datenschutz-Schutzstufe** und ist dort begründet; der BSI-Wert ist die Vorbelegung daraus.

*Sammelvermerk der Durchsicht vom 2026-08-04. In demselben Durchgang wurden 67 Speicher mit Register-, Entscheidungs- oder Gefahrenabwehrbezug angehoben; dieser gehört nicht dazu.*
