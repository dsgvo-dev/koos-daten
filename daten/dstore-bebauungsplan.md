---
id: dstore-bebauungsplan
typ: datenspeicher
system: null
name: Bebauungsplan / Flächennutzungsplan
datenkategorie: Bescheid / Nachweis
zuständige-einheit: oe-amt-61
bpmn:
  typ: datenspeicher
klassifizierung:
  schutzstufe: A
  schutzbedarf: normal
  vertraulichkeit: öffentlich
  rechtsgrundlagen:
  - gesetz: BauGB
    artikel: §8
    titel: Bebauungsplan
  - gesetz: BauGB
    artikel: §5
    titel: Flächennutzungsplan
  - gesetz: NBauO
    artikel: §63
    titel: Prüfung planungsrechtlicher Zulässigkeit
  aufbewahrung:
    frist: dauerhaft (öffentliche Satzung)
    beginn: null
    hinweis: Bebauungspläne sind öffentliche Satzungen; kein Ablaufdatum
letzte-aktualisierung: 2026-04-07
---

# Bebauungsplan / Flächennutzungsplan

## Definition

Verbindliche städtebauliche Planungsdokumente der Gemeinde. Der Bebauungsplan setzt
die Art und das Maß der baulichen Nutzung eines Gebiets fest (§ 8 BauGB); der
Flächennutzungsplan ist das übergeordnete, nicht unmittelbar verbindliche Dokument.

Im BPMN-Sinne sind sie **Data Stores**: Sie werden von mehreren Prozessen referenziert
(Baugenehmigungsverfahren, Bauvoranfrage, Befreiungsantrag), ohne selbst Teil des
Prozessflusses zu sein. Zuständig für ihre Pflege ist das Stadtplanungsamt (oe-amt-61),
nicht das Bauamt.

## Verwendung im Baugenehmigungsverfahren

Das Bauamt prüft bei jedem Bauantrag die planungsrechtliche Zulässigkeit anhand des
geltenden Bebauungsplans. Liegt kein Bebauungsplan vor, richtet sich die Zulässigkeit
nach §34 oder §35 BauGB (Innen-/Außenbereich).

## Hinweise

Bebauungspläne sind öffentlich einsehbar (§ 10 Abs. 3 BauGB). Änderungen erfordern
ein formelles Planänderungsverfahren mit Öffentlichkeitsbeteiligung.
