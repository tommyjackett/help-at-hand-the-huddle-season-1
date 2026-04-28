# The Huddle — Season 1

A Vidpod-built journey page for **Help at Hand**'s Season 1 of *The Huddle* podcast.

**Live URL** (once Pages is enabled): <https://tommyjackett.github.io/help-at-hand-the-huddle-season-1/>

## What this is

Five conversations Megan Harvey (Help at Hand founder, Emergency Clinical Nurse Educator) had with experts so members don't have to Google at 2am.

| # | Guest | Field | Episode |
| --- | --- | --- | --- |
| 1 | Claire Maule | Women's Health Physiotherapy · Pelvic Floor | 28m |
| 2 | Bianca Burge | Sleep Consultant · Midwife | 22m |
| 3 | Isabelle "Belle" Sayers | Oral Health Therapist | 26m |
| 4 | Olivia McArthur | Paediatric Dietitian | 40m |
| 5 | Felicity Conlan | Speech Pathologist · Author | 22m |

## How it works

- **Single-file `index.html`**, data-driven from `season-data.json`.
- All assets in `assets/` — heroes, BTS, fonts (GT Walsheim), brand marks, HAH stickers.
- **No build step**. Push to `main` → GitHub Pages serves it.
- **YouTube IFrame Player API** powers click-a-question-→-jump-to-the-moment seeking, with `endSeconds` to stop cleanly at the end of each answer.
- **Search** indexes every question, quote and topic — type anything (CPR, sleep, fevers, choking) and jump straight to the relevant moment.

## Schema

`season-data.json` validates against `Tools/Podcast Season Page/season-schema.json` (v0.1).

## Repo structure

```
.
├── index.html              ← the whole page (single file)
├── season-data.json        ← all content for this season (5 episodes, 25 topics, 53 questions, 15 quotes)
├── README.md               ← this file
└── assets/
    ├── brand/              ← Help at Hand symbol + lockup (also used by The Huddle wordmark)
    ├── fonts/              ← GT Walsheim (Regular / Medium / Bold / Bold-Oblique)
    ├── stickers/           ← HAH sticker library subset (Asterix in 5 colors + Heart + Bandaid + Flower)
    ├── heroes/             ← 6 hero portraits (Megan + 5 guests), compressed
    └── bts/                ← per-guest behind-the-scenes photos, compressed
```

## Brand systems (do not mix)

- **The Huddle** — pink wordmark `#EA559E`, GT Walsheim Bold, soft pink `#E0CBE1` surfaces. Used for podcast moments.
- **Help at Hand (parent)** — red circular lockup, sticker library, Futura/Emmeline. Used for "made for / by" footer credit and decorative motifs.

The Huddle is a pink room *inside* the Help at Hand house.

## Built by

[Vidpod](https://vidpod.com.au) for [Help at Hand Education](https://www.helpathandeducation.com.au).
