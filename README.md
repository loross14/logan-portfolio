# logan-portfolio

Single-file portfolio for Logan Christopher Ross. Zero dependencies, zero build step. One terminal hiding behind a backtick.

- **Stack:** one `index.html` — embedded CSS + vanilla JS. Only external resource is Google Fonts (IBM Plex Mono, Cormorant Garamond).
- **Interaction:** press `` ` `` to open an in-page terminal. Commands: `help`, `about`, `stack`, `contact`, `theme`, `clear`, `exit`, `secret`.
- **Easter eggs:** triple-click the name, the Konami code, and `secret`.

## Deploy (Vercel via GitHub)

This repo is a static site — Vercel needs no build config.

1. Push to GitHub (done).
2. On vercel.com → **Add New → Project → Import** this repo.
3. Framework preset: **Other**. Build command: *(none)*. Output directory: `./`.
4. Deploy. Every push to `main` ships automatically.

`vercel.json` sets clean URLs and security headers.
