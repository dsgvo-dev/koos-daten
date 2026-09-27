---
id: proc-gurtanlege-und-helmtragepflicht-ausnahmegenehmigung
titel: 'Gurtanlege- und Helmtragepflicht: Ausnahmegenehmigung erteilen'
status: aktiv
zustaendigeEinheit: oe-amt-34
zustaendigeRolle: ''
beteiligte:
- einheit: oe-amt-20
  aufgabe: 'Fachliche Stellungnahme zur Verkehrssicherheit (§ 46 StVO)'
daten:
  input: []
  output: []
  datenspeicher:
  - id: dstore-ausnahmegenehmigung-schwerverkehr
  - id: dstore-kfz-daten
  - id: dstore-personenstammdaten
  - id: dstore-identitaetsnachweis
  - id: dstore-gesundheitsdaten
regelungen:
- § 21a StVO (Sicherheitsgurt- und Schutzhelmpflicht)
- § 46 StVO (Ausnahmegenehmigungen)
- § 47 StVO (örtliche Zuständigkeit der Straßenverkehrsbehörde)
- VwV-StVO Rn. 93 ff. (Ausnahmegenehmigungen — Ermessensausübung, Befristung, Auflagen)
leika_id: '99108025001000'
ozg_id: null
letzte-aktualisierung: '2026-09-27'
fim_aenderung: '2026-09-16'
---
# Gurtanlege- und Helmtragepflicht: Ausnahmegenehmigung erteilen

## Prozessschritte

**01 Antrag entgegennehmen und Vollständigkeit prüfen**
*Antragstellende Person reicht formlosen oder formgebundenen Antrag mit Begründung ein (gesundheitliche Gründe, berufliche Erfordernisse). Zuständige Stelle prüft Eingang und Vollständigkeit der Unterlagen; ggf. Nachforderung fehlender Nachweise.*

**02 Ärztliches Attest / Befreiungsgründe prüfen**
*Ärztliches Gutachten oder fachärztliche Bescheinigung über die Befreiungsgründe (z. B. Wirbelsäulenerkrankung, krankhafte Adipositas, orthopädische Kontraindikation) wird auf Plausibilität und Aktualität geprüft. Bei beruflichen Gründen: Nachweis der betrieblichen Notwendigkeit (z. B. häufiges Ein- und Aussteigen bei Kurzstrecken).*

**03 Sachprüfung nach § 46 StVO i. V. m. VwV-StVO Rn. 93 ff.**
*Prüfung der Ausnahmevoraussetzungen: Verhältnismäßigkeit der Beschwer durch die Gurt-/Helmpflicht, keine Gefährdung anderer Verkehrsteilnehmer, kein milderes Mittel. Ermessensausübung nach VwV-StVO Rn. 93 ff. — Abwägung zwischen Individualinteresse und Schutzgut Verkehrssicherheit.*

**04 Beteiligung Straßenverkehrsbehörde (Amt 20)**
*Fachliche Stellungnahme zur Vereinbarkeit der Ausnahmegenehmigung mit der Verkehrssicherheit einholen (§ 47 StVO — örtliche Zuständigkeit).*

**05 Bescheid erteilen**
*Bewilligungs- oder Ablehnungsbescheid mit Rechtsbehelfsbelehrung. Bei Bewilligung: räumlich/zeitlich beschränkte Ausnahmegenehmigung mit Auflagen (z. B. nur für bestimmte Fahrzeugklassen, nur im Stadtgebiet, Befristung auf 1–3 Jahre, Mitführpflicht des Bescheids).*

**06 Auflagen überwachen und Befristung kontrollieren**
*Stichprobenartige Kontrolle, ob Auflagen eingehalten werden. Vor Ablauf der Befristung: Prüfung, ob Verlängerungsantrag erforderlich. Bei Wegfall der Befreiungsgründe: Widerruf der Ausnahmegenehmigung.*

## FIM-Änderungen (16.09.2026)

Gegenüber dem vorherigen Stand (2026-07-10) wurden folgende Änderungen aus dem aktualisierten FIM-Leistungssteckbrief 99108025001000 (Status Gold, 16.09.2026) eingearbeitet:
- § 47 StVO (örtliche Zuständigkeit) als zusätzliche Handlungsgrundlage aufgenommen
- VwV-StVO Rn. 93 ff. (Ermessensausübung, Befristung, Auflagen) als Auslegungshilfe ergänzt
- Datenspeicher `dstore-gesundheitsdaten` für das ärztliche Attest aufgenommen
- Prozessschritte von generischem Template auf spezifischen Verfahrensablauf umgestellt (ärztliches Attest, Ermessensausübung nach VwV-StVO, Befristungskontrolle)
- Duplikat `proc-ausnahmegenehmigung-gurtanlege-und-helmtragepflicht` konsolidiert (zwei Prozesse für dieselbe LeiKa-ID); Beteiligung Amt 20 aus dem gelöschten Prozess übernommen