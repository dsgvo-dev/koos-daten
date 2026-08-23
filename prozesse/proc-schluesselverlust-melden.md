---
id: proc-schluesselverlust-melden
titel: Schlüsselverlust melden
status: aktiv
zustaendigeEinheit: oe-amt-10
zustaendigeRolle: Sachbearbeitung
beteiligte:
  - einheit: oe-amt-15
    aufgabe: Sperrung elektronischer Schlüssel (Transponder, Chipkarten), Deaktivierung der Berechtigung
  - einheit: oe-hvb
    aufgabe: Entscheidung über Umstellung der Schließanlage bei Verlust von Haupt-/Generalschlüsseln
daten:
  input:
    - Meldung des Schlüsselverlusts (Name, Schlüsselnummer, Ort/Zeitpunkt des Verlusts)
  output:
    - Eintrag im Schlüsselverlustregister, Sperr-/Umstellungsnachweis
  datenspeicher:
    - id: dstore-schluesselverwaltung
    - id: dstore-vollmacht-vertretung-berechtigung
regelungen:
  - "Dienstanweisung Schlüsselverwaltung (Hausrecht)"
  - "Sicherheitsrichtlinie Gebäude (Zutrittskontrolle)"
  - "§ 86 NKomVG (Verwaltungsorganisation)"
  - "Art. 6 Abs. 1 lit. e DSGVO, § 3 NDSG (Aufgabenerfüllung)"
leika_id: null
ozg_id: null
letzte-aktualisierung: '2026-08-22'
---
# Schlüsselverlust melden

## Zweck

Meldung und Bearbeitung des Verlusts eines Dienstschlüssels oder Transponders. Die beschäftigte Person meldet den Verlust unverzüglich beim Hauptamt (oe-amt-10); dieses sperrt den Schlüssel, dokumentiert den Verlust im Schlüsselverlustregister und veranlasst bei Bedarf die Umstellung der Schließanlage. Der Prozess dient der Zutrittskontrolle und der Sicherheit der Gebäude und der darin verarbeiteten Daten.

**Anlaufstelle bei Schlüsselverlust:** Hauptamt, oe-amt-10, Sachbearbeitung — unverzüglich melden (telefonisch und schriftlich). Bei Verlust eines Haupt- oder Generalschlüssels zusätzlich die Behördenleitung (oe-hvb) informieren.

## Prozessschritte

**01 Verlust unverzüglich melden**
*Die oder der Beschäftigte meldet den Schlüsselverlust unverzüglich beim Hauptamt (oe-amt-10, Sachbearbeitung). Die Meldung erfolgt telefonisch zur Sofortsperrung und schriftlich zur Dokumentation. Angegeben werden Name, Schlüsselnummer oder Transponder-ID, Ort und Zeitpunkt des Verlusts sowie die Umstände (verloren, Diebstahl).*

**02 Schlüssel sperren**
*Das Hauptamt sperrt den Schlüssel sofort: Bei elektronischen Schlüsseln (Transponder, Chipkarten) deaktiviert die IT-Abteilung (oe-amt-15) die Berechtigung unverzüglich. Bei mechanischen Schlüsseln wird der Verlust im Schließplan vermerkt und eine Sperrung veranlasst.*

**03 Verlust dokumentieren**
*Das Hauptamt trägt den Verlust in das Schlüsselverlustregister ein: Schlüsselnummer, empfangende Person, Datum des Verlusts, Datum der Meldung, Sperrmaßnahmen. Der Eintrag wird in dstore-schluesselverwaltung dokumentiert.*

**04 Schließanlage umstellen (bei Bedarf)**
*Bei Verlust von Haupt- oder Generalschlüsseln entscheidet die Behördenleitung (oe-hvb) über die Umstellung der betroffenen Schließanlage. Bei einfachen Zimmer- oder Bereichsschlüsseln wird geprüft, ob eine Umstellung erforderlich ist. Die Umstellung wird dokumentiert und der neue Zylinder in das Schlüsselverzeichnis aufgenommen.*

**05 Ersatz und Strafanzeige**
*Nach der Sperrung wird dem oder der Beschäftigten auf Antrag ein Ersatzschlüssel ausgegeben (siehe proc-schluesselverwaltung, Schritt 02). Bei Diebstahl ist eine Strafanzeige zu erstatten; die Anzeige wird aktenkundig gemacht.*

**06 Rückblick und Prävention**
*Das Hauptamt prüft, ob der Verlust auf einen systematischen Mangel hindeutet (z. B. fehlende Rückgabe bei Austritten) und veranlasst bei Bedarf Nachschärfungen in der Dienstanweisung Schlüsselverwaltung.*

**Herkunft des Schrittblocks:** abgeleitet aus der Dienstanweisung Schlüsselverwaltung, der Sicherheitsrichtlinie Gebäude, § 86 NKomVG sowie Art. 6 Abs. 1 lit. e DSGVO i.V.m. § 3 NDSG, nicht aus einer Ablauferhebung im Amt 10.