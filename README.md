# Jane Street Puzzle Practice

Playable versions of [Jane Street's monthly puzzles](https://www.janestreet.com/puzzles/). Warm up on little boards until the rules click, then take on the real one.

**Play:** https://johnlam1968.github.io/jane-street-puzzle-practice/ · 中文版：https://johnlam1968.github.io/jane-street-puzzle-practice/index.zh.html

Works on iPhone, iPad, Android and desktop browsers. Each page is one self-contained HTML file with no build step. Progress is saved in the browser's local storage.

## Puzzles

| Month | Puzzle | What you get |
| --- | --- | --- |
| October 2026 | [It's a Metric, Too](https://johnlam1968.github.io/jane-street-puzzle-practice/its-a-metric-too/harness.html) | [Play](https://johnlam1968.github.io/jane-street-puzzle-practice/its-a-metric-too/harness.html) (中文版 [here](https://johnlam1968.github.io/jane-street-puzzle-practice/its-a-metric-too/harness.zh.html)): 49 practice boards (4×4 to 7×7), each with exactly one solution, plus the original 11×11 with a rule checker. The harness lets you paint the states you are assuming, assume a capitol (including a hidden one), and re-checks every published number against the real travel costs. |

## Why a website instead of the HTML file

If you send an `.html` file to an iPhone or iPad (through iMessage, AirDrop, email or Files), iOS opens it in Quick Look, and Quick Look does not run JavaScript. The page shows up blank. The same file served from a URL runs normally in Safari, which is why these pages are hosted on GitHub Pages.

## Adding a puzzle

1. Create a folder named after the puzzle, such as `my-next-puzzle/`, with an `index.html` inside. Keep everything (CSS, JS, data) in that one file.
2. Add a `← All puzzles` link pointing to `../index.html` (and to `../index.zh.html` on the Chinese page).
3. Add a card for it at the top of the list in the root `index.html` (and in `index.zh.html`), and a row at the top of the table above.
4. Commit and push to `feat/assumption-ledger`. GitHub Pages redeploys in about a minute.

To preview locally:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Disclaimer

This is an unofficial fan project and is not affiliated with Jane Street. The puzzles, their rules and the original grids belong to Jane Street. This repository only contains practice versions and checkers, not answers to open puzzles.
