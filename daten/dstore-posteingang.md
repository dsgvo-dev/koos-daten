---
id: dstore-posteingang
bereich: intern
typ: datenspeicher
system: null
name: Posteingang
zuständige-einheit: oe-amt-10
personenbezug: ja
bpmn:
  typ: datenobjekt
klassifizierung:
  # Datenschutz -- Schaden für die betroffene Person (LfD-Schutzstufenkonzept, SDM)
  schutzstufe: C
  schutzbedarf: normal
  vertraulichkeitsklasse: vertraulich
  # Informationssicherheit -- Schaden für die Institution und die Aufgabenerfüllung (BSI)
  bsi-vertraulichkeit: normal
  bsi-integritaet: normal
  bsi-verfuegbarkeit: normal
  bsi-schutzbedarf: normal
  rechtsgrundlagen:
  - gesetz: DSGVO
    artikel: Art. 6 Abs. 1 lit. e
  - gesetz: NDSG
    artikel: § 3
  - gesetz: NVwVfG
    artikel: § 1 i. V. m. § 3a VwVfG (elektronischer Zugang)
  aufbewahrung:
    frist: bis zur Weiterleitung, spätestens 3 Monate
    beginn: Eingang
    hinweis: 'Festlegung des Trägers (Entwurf Claude, Freigabe Martin 06.10.2026): Mit der Weiterleitung gehört das Schriftstück zur Akte des Fachamts; Scans und E-Mails im zentralen Postfach werden nach der Weiterleitung gelöscht, spätestens nach 3 Monaten. Kein Posteingangsbuch.'
letzte-aktualisierung: '2026-10-05'
tags:
- Poststelle
- Posteingang
- elektronische Post
---

# Posteingang

## Definition

Daten, die beim Durchlauf von Post durch die Poststelle anfallen: Papierpost und elektronische Post an das zentrale Postfach, bis zur Weiterleitung an die zuständige Organisationseinheit; Postausgang. Es wird kein Posteingangsbuch geführt.

## Felder

- Absender (Name, Anschrift oder E-Mail-Adresse)
- zuständige Organisationseinheit
- Eingangsdatum
- Art des Eingangs (Brief, E-Mail an das zentrale Postfach, sonstiger elektronischer Zugang)
- Scan oder E-Mail im zentralen Postfach bis zur Weiterleitung
- Weiterleitungsvermerk
- Postausgang: Empfänger, Versanddatum

## Hinweise

**Anlass.** Angelegt am 2026-10-05 bei der Trennung interner und externer Datenspeicher (Plan vom 05.10.2026, Schritt 7, Entscheidung Martin). `proc-poststelle` nutzte bis dahin `dstore-kontaktdaten` (extern). Entscheidung Martin 06.10.2026: eigener Speicher einschließlich elektronischer Post, kein Posteingangsbuch.

**Schutzstufe C.** Post kann Inhalte jeder Art enthalten; Sendungen mit dem Vermerk „persönlich/vertraulich“ werden ungeöffnet weitergeleitet.

**BSI-Vektoren.** Vertraulichkeit normal, Integrität normal, Verfügbarkeit normal — Die Daten liegen nur vorübergehend in der Poststelle.

**Abgrenzung:**
- `dstore-kontaktdaten`: Kontaktdaten in Bürgerverfahren, extern.
- Akten der Fachämter: Ziel der Weiterleitung, nicht Teil dieses Speichers.
