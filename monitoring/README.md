<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Beobachtung: was gelesen wird und was daraus folgte

[English](README.en.md)

Wie global-law jedes Land beobachtet: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). Diese Seite zeigt dasselbe nur für Appenzell Innerrhoden: jedes Lesen einer amtlichen Quelle, wann, und was daraus folgte (Vorschriften hinzugefügt, geändert und entfernt). Maschinenlesbar in [data/checks/](../data/checks/) (JSON Lines, Schema `lexifina-check/1`), in `git log` als Commits mit `Kind: check` und Monat für Monat in [checks/](checks/).

**Letzte Prüfung:** 2026-11-26 05:42 UTC, Appenzell Innerrhoden: Systematische Sammlung (ai.clex.ch): 154 Adressen gelesen; 0 hinzugefügt, 0 geändert, 0 entfernt; keine Änderung; 7 nicht veröffentlicht, davon 0 ohne Grund. Hinweise: `verify-differ`.

## Quellen

| Quelle | Ordner | Wie oft | Letzte erfolgreiche Prüfung | Letztes Ergebnis | Stand |
| --- | --- | --- | --- | --- | --- |
| [Appenzell Innerrhoden: Systematische Sammlung (ai.clex.ch)](https://ai.clex.ch/) | `<act>/` | täglich | 2026-11-26 05:42 UTC | keine Änderung | beobachtet |

## Die letzten 30 Tage

| Beginn (UTC) | Quelle | Gelesen | Hinzugefügt | Geändert | Entfernt | Nicht veröffentlicht (ohne Grund) | Ergebnis | Commits |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-26 05:39](checks/2026-11.md#ch-lexwork-appenzell-innerrhoden-20261126t053947z) | lexwork-appenzell-innerrhoden | 154 | 0 | 0 | 0 | 7 (0) | keine Änderung `verify-differ` | — |
| [2026-11-25 05:45](checks/2026-11.md#ch-lexwork-appenzell-innerrhoden-20261125t054516z) | lexwork-appenzell-innerrhoden | 248 | 123 | 0 | 0 | 7 (0) | Änderungen gefunden `verify-differ` | [213](https://github.com/lexifina/switzerland-appenzell-innerrhoden-law/compare/5978e889beeb...ffc23308e77b) |
| [2026-11-24 14:30](checks/2026-11.md#ch-lexwork-appenzell-innerrhoden-20261124t143026z) | lexwork-appenzell-innerrhoden | 174 | 123 | 1 | 0 | 131 (0) | die Prüfung ist fehlgeschlagen | — |
| [2026-11-24 12:54](checks/2026-11.md#ch-lexwork-appenzell-innerrhoden-20261124t125448z) | lexwork-appenzell-innerrhoden | 167 | 123 | 0 | 0 | 130 (0) | die Prüfung ist fehlgeschlagen | — |
| [2026-11-24 11:51](checks/2026-11.md#ch-lexwork-appenzell-innerrhoden-20261124t115103z) | lexwork-appenzell-innerrhoden | 493 | 130 | 0 | 0 | 135 (0) | die Prüfung ist fehlgeschlagen | — |

## Selbst prüfen

```
python tools/checktrail.py                      # die letzte Prüfung jeder Quelle
python tools/checktrail.py --day 2026-11-23     # jede Prüfung eines Tages
python tools/checktrail.py --act <id>           # wann eine Vorschrift gesehen und veröffentlicht wurde
git log --grep='^Kind: check' --format='%ci %s'  # die Prüfungen in der Historie
```

Rechtskraft hat nur die amtliche Verkündung; die Texte hier sind Kopien zum Lesen und Suchen.
