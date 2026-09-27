---
# Muster Prozess. Datei kopieren nach prozesse/proc-<kurzname>.md und alle <Platzhalter> ersetzen.
# Kommentarzeilen (#) vor dem Speichern entfernen.
id: proc-<kurzname>
# Stabile ID = Dateiname ohne .md. Präfix proc- und kebab-case: ä→ae, ö→oe, ü→ue, ß→ss. Niemals nachträglich ändern.
titel: <Titel als Tätigkeit, z. B. „Schlüsselverlust melden">
status: entwurf
# entwurf | aktiv | inaktiv | ersetzt. „aktiv" heißt: wird geführt.
zustaendigeEinheit: oe-<id>
# ID aus orga.yaml. Die Einheit, die den Prozess steuert.
zustaendigeRolle: <Rolle, z. B. Sachbearbeitung>
beteiligte:
- einheit: oe-<id>
  aufgabe: <Teilaufgabe dieser Einheit>
daten:
  input:
  - <Eingang, Freitext, z. B. Antrag mit Unterlagen>
  output:
  - <Ergebnis, Freitext, z. B. Bescheid>
  datenspeicher:
  - id: dstore-<id>
  # Nur IDs aus daten/. Die Rückverweise berechnet der Resolver; der Datenspeicher nennt keine Prozesse.
regelungen:
- reg-<id>
- <Norm als Freitext, z. B. Art. 6 Abs. 1 lit. e DSGVO, § 3 NDSG>
leika_id: null
# 14-stelliger LeiKa-Schlüssel in Anführungszeichen, sonst null.
ozg_id: null
letzte-aktualisierung: '<JJJJ-MM-TT>'
# Nur bei status ersetzt: ersetzt-durch: proc-<id>
---

# <Titel>

## Zweck

<Ein bis drei Sätze: Was leistet der Prozess, für wen, auf welcher Grundlage.>

## Prozessschritte

**01 <Schritt als Tätigkeit>**
*<Was geschieht, wer handelt, welches Ergebnis entsteht. Ein Absatz, keine harten Zeilenumbrüche.>*

**02 <Schritt als Tätigkeit>**
*<…>*

**Herkunft des Schrittblocks:** <abgeleitet aus Norm oder Regelung X / erhoben im Amt Y am JJJJ-MM-TT>
