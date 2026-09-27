# Muster für KOOS-Dateien

Stand 27.09.2026

Dieser Ordner enthält ausfüllbare Vorlagen für die vier gepflegten Dateitypen. Der Resolver liest ihn nicht, weil `koos.yaml` nur `proc-*`, `dstore-*`, `reg-*` und `vvt-*` in den Modulordnern erfasst.

| Muster | Ziel | ID-Präfix |
|--------|------|-----------|
| `muster-prozess.md` | `prozesse/` | `proc-` |
| `muster-datenspeicher.md` | `daten/` | `dstore-` |
| `muster-vvt.md` | `vvt/` | `vvt-` |
| `muster-regelung.md` | `regelungen/` | `reg-` |

## Anwendung

1. Muster in den Zielordner kopieren und nach der neuen ID benennen.
2. Alle `<Platzhalter>` ersetzen und die Kommentarzeilen (`#`) entfernen.
3. Verweise nur auf IDs setzen, die es gibt (`oe-` aus `orga.yaml`, `dstore-`, `proc-`, `reg-`).
4. Jeden Absatz auf eine Zeile schreiben; keine harten Zeilenumbrüche im Fließtext.

## Festlegungen, die die Muster treffen

- **Maßgeblich ist der Bestand, nicht das README von KOOS.** Das README beschreibt die Datenspeicher noch mit einer Klassifizierungsachse und kennt die VVT nicht.
- **Regelungen:** Feldname `entscheidendes-gremium` (Schreibweise des README und von 17 der 26 Regelungen). Der Server liest beide Schreibweisen.
- **Statuswerte:** Prozess `entwurf | aktiv | inaktiv | ersetzt`; VVT `aktiv | inaktiv`; Regelung `entwurf | aktiv | aufgehoben` (koos.yaml, Hinweis zum Feld `status`).
- **TOM:** In der VVT bleibt `tom: []`. Die Maßnahmen stehen in `tom/tom-<vvt-id>.json` und werden erzeugt.
- **Nicht vorgesehen:** Die ADR-Felder `kontext`, `entscheidung` und `alternativen` aus dem README nutzt keine Regelung im Bestand; die Muster führen sie nicht.

## Texte von Dienstvereinbarungen und Dienstanweisungen

Den Inhalt liefern die Muster im DSMS:

- `dsms-knowledge/facts/muster/Muster-Dienstvereinbarung-allgemein.md`
- `dsms-knowledge/facts/muster/dienstanweisungen/Muster-Dienstanweisung-allgemein.md`
