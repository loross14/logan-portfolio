# logan-portfolio

Portfolio for Logan Christopher Ross. Two surfaces over one body of work. Zero dependencies, zero build step.

## Surfaces

- **`/` — the hero + terminal.** One `index.html`, embedded CSS + vanilla JS. Press `` ` `` to open an in-page terminal.
  - Commands: `help`, `about`, `stack`, `contact`, `theme`, `clear`, `exit`, `secret`.
  - **The body — a knowledge graph of the work:** `body` (the eight repositories), `books <repo>`, `open <id>`, `findings`, `links <id>`, `read`.
  - Easter eggs: triple-click the name, the Konami code, `secret`.
- **`/body` — the narrative.** `body.html`, the findings glossed: the same κ in whales and tumors, the Copper Scroll, the 15-script ledger. Its doors deep-link back into the live graph (`/?open=<id>`).

## The knowledge graph

The terminal navigates a self-contained graph of **8 repositories, 73 research books, and 4 cross-domain findings** (κ, treewidth, the script ledger, the Copper Scroll), inlined into `index.html` so the site stays single-file and works from `file://`.

The eight constellation repositories are **private — available by request**; the graph carries the findings as data and never links to a private repo (no 404 doors). It is generated from forge canon by `state/graph/build-graph.py`, which also injects the public projection between the `/*GRAPH:START*/…/*GRAPH:END*/` markers.

Deep links: `/?open=<id>` opens the terminal to a node; `/?cmd=<command>` runs any command.

## Deploy (Vercel via GitHub)

This repo is a static site — Vercel needs no build config.

1. Push to GitHub (done).
2. On vercel.com → **Add New → Project → Import** this repo.
3. Framework preset: **Other**. Build command: *(none)*. Output directory: `./`.
4. Deploy. Every push to `main` ships automatically.

`vercel.json` sets clean URLs and security headers.
