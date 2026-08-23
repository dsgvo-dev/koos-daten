---
id: proc-austritt-beendigung-beschaeftigungsverhaeltnis
titel: Austritt / Beendigung des Beschäftigungsverhältnisses
status: aktiv
zustaendigeEinheit: oe-amt-11
zustaendigeRolle: Sachbearbeitung
beteiligte:
  - einheit: oe-amt-15
    aufgabe: IT-Zugänge sperren, E-Mail-Konto deaktivieren, Dienstgeräte entgegennehmen
  - einheit: oe-hvb
    aufgabe: Entlassungsurkunde unterzeichnen (Beamte), Kündigungsschreiben zeichnen
  - einheit: oe-personalrat
    aufgabe: Anhörung/Mitbestimmung nach §§ 64–67 NPersVG
  - einheit: oe-amt-1-4
    aufgabe: Anordnung der Löschung personenbezogener Daten nach Ablauf der Aufbewahrungsfrist
daten:
  input:
    - Kündigungsschreiben, Rentenantrag, Resturlaubsnachweis, Dienstausweis, Schlüssel
  output:
    - Entlassungsurkunde, Arbeitszeugnis, letzte Abrechnung, Rentenauskunft, Löschprotokoll
  datenspeicher:
    - id: dstore-personalakte
    - id: dstore-arbeitsverhaeltnis-beschaeftigung
    - id: dstore-it-berechtigungsantrag
    - id: dstore-abrechnungsdaten
    - id: dstore-rentenversicherungsverlauf
regelungen:
  - "Art. 88 DSGVO i.V.m. § 12 NDSG (Beschäftigtendatenschutz)"
  - "§§ 88, 94 NBG (Personalakte, Gesundheitsdaten)"
  - "§ 50 BeamtStG (Personalakte)"
  - "§§ 41, 47 BeamtStG (Entlassung, Ruhestand)"
  - "§§ 34–37 TVöD/TV-L (Kündigung des Arbeitsverhältnisses)"
  - "§§ 64–67 NPersVG (Mitbestimmung des Personalrats)"
  - "§ 195 BGB (Regelverjährung als Aufbewahrungsfrist)"
  - "§ 147 AO (steuerliche Aufbewahrungsfristen)"
  - "§ 109 GewO (Anspruch auf Arbeitszeugnis)"
  - "§ 86 NKomVG (Personalhoheit)"
leika_id: null
ozg_id: null
letzte-aktualisierung: '2026-08-21'
---
# Austritt / Beendigung des Beschäftigungsverhältnisses

## Zweck

Der Prozess umfasst alle Schritte zwischen dem Auslöser der Beendigung (Kündigung, Aufhebungsvertrag, Ruhestandseintritt, Ablauf der Probezeit oder Tod) und dem vollständigen Abschluss des Beschäftigungsverhältnisses: Abwicklung der Personalakte, Zeugniserteilung, letzte Abrechnung, Rückgabe von Dienstmitteln, Sperrung von IT-Zugängen und Datenlöschung nach Ablauf der Aufbewahrungsfristen. Betroffen sind alle ausscheidenden Beamtinnen und Beamten sowie Tarifbeschäftigte einschließlich Auszubildender. Das Arbeitszeugnis wird im Teilprozess `proc-zeugnis-ausstellen` gesondert behandelt.

## Prozessschritte

**01 Beendigungserklärung und Fristenprüfung**
*Eingang der Kündigung, des Aufhebungsvertrags oder der Mitteilung über den Ruhestandseintritt. Die Personalabteilung prüft die Einhaltung der Kündigungsfrist (§§ 34–37 TVöD, §§ 30–33 NBG i.V.m. BeamtStG), die Schriftform (§§ 126, 623 BGB) und bei Kündigung durch die Behörde die vorherige Anhörung des Personalrats nach § 66 Abs. 1 Nr. 6 NPersVG.*

**02 Personalrat anhören (bei Kündigung durch die Behörde)**
*Vor Ausspruch einer Kündigung oder einer Entlassung wird der Personalrat nach § 66 Abs. 1 Nr. 6 NPersVG angehört. Die Anhörung ist aktenkundig zu machen. Bei mitbestimmungspflichtigen Begleitumständen (Aufhebungsvertrag mit Abfindung, Sondervereinbarungen) ist § 64 NPersVG zu beachten. Bei schwerbehinderten Beschäftigten erfolgt zusätzlich die Beteiligung der Schwerbehindertenvertretung nach § 178 Abs. 2 SGB IX.*

**03 Resturlaub und Freistellung klären**
*Die Personalabteilung ermittelt den Resturlaubsanspruch. Offene Urlaubstage sind innerhalb der Kündigungsfrist zu gewähren oder nach § 7 Abs. 4 BUrlG abzugelten. Bei Freistellung wird die Dauer und die Anrechnung auf den Resturlaub schriftlich festgehalten.*

**04 Zeugnis und Entlassungsurkunde**
*Die Personalabteilung leitet die Zeugniserstellung nach § 109 GewO (einfaches oder qualifiziertes Arbeitszeugnis) ein — siehe `proc-zeugnis-ausstellen`. Bei Beamtinnen und Beamten wird die Entlassungsurkunde nach § 41 BeamtStG durch die Behördenleitung (oe-hvb) unterzeichnet. Bei Ruhestand tritt an die Stelle der Entlassung die Versetzung in den Ruhestand nach § 47 BeamtStG.*

**05 Letzte Abrechnung und Rentenauskunft**
*Die abrechnende Stelle erstellt die letzte Gehalts-/Lohnabrechnung, berechnet die Abgeltung von Resturlaub und Überstunden und führt die Auszahlung des Guthabens durch. Für die Rentenversicherung wird die Pflichtabfrage nach § 109 SGB VI durchgeführt und eine Rentenauskunft erstellt. Die Abrechnungsdaten werden in der dstore-abrechnungsdaten dokumentiert.*

**06 IT-Zugänge sperren und Dienstgeräte zurücknehmen**
*Die IT-Abteilung (oe-amt-15) sperrt alle Zugriffsberechtigungen zum Austrittsdatum: Fachverfahren, E-Mail-Konto, Netzwerkzugang, VPN und Dateiverzeichnisse. Die Dienstgeräte (Laptop, Diensthandy) werden entgegengenommen, auf Werkszustand zurückgesetzt und der Berechtigungsantrag in der dstore-it-berechtigungsantrag geschlossen.*

**07 Dienstausweis, Schlüssel und Unterlagen zurücknehmen**
*Die Personalabteilung nimmt den Dienstausweis, die Schlüssel, die Parkkarte sowie alle dienstlichen Unterlagen entgegen. Die Rückgabe wird dokumentiert. Bei Verlust wird ein Verlustvermerk aufgenommen.*

**08 Personalakte schließen und aufbewahren**
*Die Personalakte wird nach § 88 NBG mit einem Abschlussvermerk versehen, der den Austrittsgrund, das Austrittsdatum und den Verbleib der Akte dokumentiert. Die Personalakte unterliegt der Aufbewahrungsfrist von zehn Jahren nach Austritt (§ 195 BGB i.V.m. § 88 NBG); steuerlich relevante Unterlagen werden nach § 147 AO sechs Jahre aufbewahrt. Nach Fristablauf wird die Löschung oder Archivierung nach dem Löschkonzept der Verwaltung veranlasst. Die Löschung wird in einem Löschprotokoll dokumentiert (Rechenschaftspflicht Art. 5 Abs. 2 DSGVO).*

**Herkunft des Schrittblocks:** abgeleitet aus §§ 88, 94 NBG, § 50 BeamtStG, §§ 41, 47 BeamtStG, §§ 34–37 TVöD/TV-L, §§ 64–67 NPersVG, § 109 GewO, Art. 88 DSGVO i.V.m. § 12 NDSG sowie § 195 BGB, nicht aus einer Ablauferhebung im Amt 11.