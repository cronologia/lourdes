# Nossa Senhora de Lourdes — Cronologia

An open, source-referenced chronology of the apparitions reported by
Bernadette Soubirous at the Massabielle grotto in Lourdes, France, in 1858,
and of the documented acts of the Catholic Church concerning them — from
Pius IX's *Ineffabilis Deus* (1854) through Bishop Laurence's recognition
decree (1862) to the bishop-declared recognitions of cures that continue
today.

**Site:** https://cronologia.github.io/lourdes/ (en / es / pt)

Part of the [Cronologia](https://github.com/cronologia) project family.

## Sourcing posture

The apparitions are recorded as **reported** events: the dataset states who
reported what and when, and what the Church ruled and when, citing the ruling
document. It never asserts the supernatural claim as fact. Church-approval
status is a first-class, dated, attributed field (Bishop Laurence's decree of
18 January 1862). Cure counts are attributed to the Sanctuary of Lourdes, and
the datable events recorded are the bishops' acts of recognition — never
"X miracles happened". See `AGENTS.md` and the `sourcing-rules` skill in
`cronologia/core`.

## How it works

```
data/chronology.json   source of truth (English, hand-edited, every entry cited)
data/i18n/{es,pt}.json committed translation dictionaries (hand-authored)
build.js               zero-dependency compiler -> docs/{en,es,pt}/
docs/                  compiled static site, served by GitHub Pages
```

Edit the data, then run the gate and commit data + regenerated `docs/`
together:

```
node scripts/validate-data.js && node --test && node build.js
```

## Contributing

Corrections against primary sources are welcome via pull request. Every fact
needs a citation; uncertain dates carry `dateVerified: false` and a
`dateNote` saying how the sources disagree.
