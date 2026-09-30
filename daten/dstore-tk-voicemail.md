---
id: dstore-tk-voicemail
typ: datenspeicher
system: null
name: Voice-Mail (Sprachspeicher)
zuständige-einheit: oe-amt-15
bpmn:
  typ: datenspeicher
klassifizierung:
  # Datenschutz -- Schaden fuer die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: D
  schutzbedarf: hoch
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden fuer die Institution und die Aufgabenerfuellung (BSI)
  bsi-vertraulichkeit: hoch
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: hoch
  rechtsgrundlagen:
  - gesetz: Art. 88 DSGVO i.V.m. § 12 NDSG
  - gesetz: Art. 6 Abs. 1 lit. e DSGVO i.V.m. § 14 NDSG
  - gesetz: § 3 TDDDG
  - gesetz: Dienstvereinbarung Telekommunikationsanlagen (reg-dv-telefonie)
  aufbewahrung:
    frist: bis zur Löschung durch den Benutzer
    beginn: Eingang der Nachricht
letzte-aktualisierung: '2026-09-30'
tags:
- Telefonie
- Voice-Mail
- Kommunikationsinhalt
---

# Voice-Mail (Sprachspeicher)

## Definition

Im Sprachspeicher der Telekommunikationsanlage hinterlassene Nachrichten von
internen und externen Anrufenden. Es sind Kommunikationsinhalte.

## Felder

- Sprachnachricht (Audio)
- Rufnummer der anrufenden Person, soweit übermittelt
- Datum und Uhrzeit des Eingangs
- Ziel-Nebenstelle

## Rechtsgrundlage

Art. 88 DSGVO i.V.m. § 12 NDSG (Beschäftigte); Art. 6 Abs. 1 lit. e DSGVO
i.V.m. § 14 NDSG (externe Anrufende); § 3 TDDDG (Fernmeldegeheimnis);
Dienstvereinbarung Telekommunikationsanlagen (`reg-dv-telefonie`) § 3 Abs. 4.

## Löschfrist

Bis zur Löschung durch den Benutzer (DV § 3 Abs. 4; `vvt-1-5-001`).

## Verwendung in Prozessen

- (wird automatisch befüllt)

## Hinweise

Nur berechtigte Nutzer dürfen die Nachrichten abhören (DV § 3 Abs. 4).

## Schutzstufe geprüft 2026-09-30

**D.** Der Inhalt ist nicht vorhersehbar. Typisch sind Krankmeldungen von
Beschäftigten und Anliegen von Bürgerinnen und Bürgern — also regelmäßig
Gesundheitsdaten (Art. 9 DSGVO) und Sozialdaten, die das Schutzstufenkonzept
als Beispiele für D nennt. Nicht E: kein regelmäßiger Bezug zu Gefahren für
Leib, Leben oder Freiheit.

*Quelle: `vvt-1-5-001` (Datenkategorie „Voice-Mail-Nachrichten“),
`reg-dv-telefonie` §§ 3, 9 Abs. 1.*
