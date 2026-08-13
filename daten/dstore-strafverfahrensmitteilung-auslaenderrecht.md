---
id: dstore-strafverfahrensmitteilung-auslaenderrecht
typ: datenspeicher
system: null
name: Strafverfahrensmitteilung an die Ausländerbehörde
datenkategorie: Migration & Aufenthalt
zuständige-einheit: oe-amt-47
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
    artikel: Art. 10
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. c
  - gesetz: NDSG
    artikel: § 17
  - gesetz: AufenthG
    artikel: § 87 Abs. 2
  - gesetz: AufenthG
    artikel: § 87 Abs. 4
  aufbewahrung:
    frist: wie die Ausländerakte
    beginn: nach Abschluss des aufenthaltsrechtlichen Verfahrens
    hinweis: Die Mitteilung ist Teil der Ausländerakte und teilt deren Frist. Nach
      Tilgung der zugrunde liegenden Eintragung im Bundeszentralregister darf sie
      nicht mehr zum Nachteil der betroffenen Person verwertet werden.
letzte-aktualisierung: '2026-08-10'
tags:
- Aufenthaltsrecht
- Art. 10 DSGVO
- Strafverfahren
---



# Strafverfahrensmitteilung an die Ausländerbehörde

## Definition

Mitteilungen anderer öffentlicher Stellen an die Ausländerbehörde über Straf- und Bußgeldverfahren sowie über sonstige Ausweisungsgründe.

## Felder

- Betroffene Person
- mitteilende Stelle und Datum
- Art der Mitteilung nach § 87 AufenthG
- Einleitung des Strafverfahrens
- Erhebung der öffentlichen Klage
- Erlass, Aufhebung oder Aussetzung eines Haftbefehls
- Erledigung des Verfahrens mit angewandter Vorschrift
- Einleitung eines Auslieferungsverfahrens
- Verwertung im aufenthaltsrechtlichen Verfahren

## Hinweise

Angelegt am 2026-08-03 zu `vvt-47-001` (Aufenthaltsrecht).

**Datum nach Art. 10 DSGVO.** § 87 Abs. 4 AufenthG verpflichtet die für Straf- und Bußgeldverfahren zuständigen Stellen, die Ausländerbehörde unverzüglich über die **Einleitung** des Strafverfahrens und über dessen **Erledigung** unter Angabe der gesetzlichen Vorschriften zu unterrichten. Entsprechendes gilt für die Erhebung der öffentlichen Klage, für Erlass, Aufhebung und Aussetzung eines Haftbefehls sowie für die Einleitung eines Auslieferungsverfahrens. § 87 Abs. 2 AufenthG erfasst darüber hinaus Mitteilungen über sonstige Ausweisungsgründe.

**Die Unschuldsvermutung ist ein Feld, keine Fußnote.** Mitgeteilt wird bereits die **Einleitung** eines Verfahrens -- also zu einem Zeitpunkt, zu dem über Schuld nichts feststeht. Deshalb führt der Speicher Einleitung und Erledigung getrennt: Wird ein Verfahren eingestellt, muss das in derselben Akte sichtbar sein wie seine Einleitung. Eine Ausländerakte, die nur den Anfangsverdacht kennt, ist unrichtig im Sinne des Art. 5 Abs. 1 lit. d) DSGVO.

**Die betroffene Person erfährt davon nicht von sich aus.** Die Mitteilung erfolgt zwischen Behörden; Art. 14 DSGVO ist zu beachten, soweit keine Beschränkung nach § 8 NDSG greift.

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
