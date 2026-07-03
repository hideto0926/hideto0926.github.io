# hpTop — Apps index / アプリ一覧トップ

Bilingual (EN / 日本語) landing page that introduces all of hideto's apps and
links to each app's own GitHub Pages site.

Live (after deploy): https://hideto0926.github.io/hpTop/

## Files
- `index.html` — the index page (inline CSS/JS, no build step)
- `assets/` — app icons used on the cards
- `.nojekyll` — serve files as-is on GitHub Pages

## Apps & links
| App | Page (GitHub Pages) | App Store |
|-----|---------------------|-----------|
| superMosaic   | https://hideto0926.github.io/superMosaic/ | https://apps.apple.com/jp/app/supermosaic/id6778454220 |
| BeatShuffle   | https://hideto0926.github.io/BeatShuffle/ | https://apps.apple.com/jp/app/beatshuffle/id6778877123 |
| Barcode Pocket| https://hideto0926.github.io/barcodeClip/ | — |
| 麻雀EYE        | https://hideto0926.github.io/MahjongEye/  | — |
| 30minTimer    | https://hideto0926.github.io/30minTimer/  | — |

## Deploy (GitHub Pages)
1. Push the contents of this folder to the **root** of the `hpTop` repo
   (https://github.com/hideto0926/hpTop), default branch.
2. Repo → Settings → Pages → Source: *Deploy from a branch* → branch = default, folder = `/ (root)`.
3. Wait ~1 min, then open https://hideto0926.github.io/hpTop/.

## Notes
- Adding a new app: copy a `<article class="card">` block in `index.html`, drop its
  icon in `assets/`, and update the link. Use `badge live` for App Store apps,
  `badge web` for ones not yet on the store.
- Language defaults to the visitor's browser language and can be toggled top-right;
  the choice is remembered via `localStorage`.
