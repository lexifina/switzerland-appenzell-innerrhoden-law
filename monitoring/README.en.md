<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Monitoring: what is read and what came of it

[Deutsch](README.md)

How global-law monitors every country: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). This page is the same for Appenzell Innerrhoden only: every time an official source is read, when, and what came of it (acts added, changed and removed). The machine-readable form is [data/checks/](../data/checks/) (JSON Lines, schema `lexifina-check/1`), in `git log` as `Kind: check` commits, and month by month in [checks/](checks/).

**Last check:** 2026-11-28 05:42 UTC, Appenzell Innerrhoden: systematic collection (ai.clex.ch): 130 addresses read; 0 added, 0 changed, 0 removed; no change; 7 not published, 0 of them with no reason. Flags: `verify-differ`.

## Sources

| Source | Folders | How often | Last successful check | Last result | State |
| --- | --- | --- | --- | --- | --- |
| [Appenzell Innerrhoden: systematic collection (ai.clex.ch)](https://ai.clex.ch/) | `<act>/` | daily | 2026-11-28 05:42 UTC | no change | watched |

## The last 30 days

| Started (UTC) | Source | Read | Added | Changed | Removed | Not published (no reason) | Result | Commits |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-28 05:40](checks/2026-11.md#ch-lexwork-appenzell-innerrhoden-20261128t054021z) | lexwork-appenzell-innerrhoden | 130 | 0 | 0 | 0 | 7 (0) | no change `verify-differ` | — |
| [2026-11-27 05:41](checks/2026-11.md#ch-lexwork-appenzell-innerrhoden-20261127t054121z) | lexwork-appenzell-innerrhoden | 143 | 0 | 1 | 0 | 9 (0) | changes found `verify-differ` | — |
| [2026-11-26 05:39](checks/2026-11.md#ch-lexwork-appenzell-innerrhoden-20261126t053947z) | lexwork-appenzell-innerrhoden | 154 | 0 | 0 | 0 | 7 (0) | no change `verify-differ` | — |
| [2026-11-25 05:45](checks/2026-11.md#ch-lexwork-appenzell-innerrhoden-20261125t054516z) | lexwork-appenzell-innerrhoden | 248 | 123 | 0 | 0 | 7 (0) | changes found `verify-differ` | [213](https://github.com/lexifina/switzerland-appenzell-innerrhoden-law/compare/5978e889beeb...ffc23308e77b) |
| [2026-11-24 14:30](checks/2026-11.md#ch-lexwork-appenzell-innerrhoden-20261124t143026z) | lexwork-appenzell-innerrhoden | 174 | 123 | 1 | 0 | 131 (0) | the check failed | — |
| [2026-11-24 12:54](checks/2026-11.md#ch-lexwork-appenzell-innerrhoden-20261124t125448z) | lexwork-appenzell-innerrhoden | 167 | 123 | 0 | 0 | 130 (0) | the check failed | — |
| [2026-11-24 11:51](checks/2026-11.md#ch-lexwork-appenzell-innerrhoden-20261124t115103z) | lexwork-appenzell-innerrhoden | 493 | 130 | 0 | 0 | 135 (0) | the check failed | — |

## Check it yourself

```
python tools/checktrail.py                      # the latest check of every source
python tools/checktrail.py --day 2026-11-23     # every check of a day
python tools/checktrail.py --act <id>           # when an act was seen and published
git log --grep='^Kind: check' --format='%ci %s'  # the checks in the history
```

Only the official publication has legal force; the texts here are copies for reading and searching.
