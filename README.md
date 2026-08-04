# hpTop — Apps index / アプリ一覧トップ

Bilingual (EN / 日本語) landing page that introduces all of hideto's apps and
links to each app's own GitHub Pages site.

Live (after deploy): https://hideto0926.github.io/hpTop/

## Files
- `index.html` — the index page (inline CSS/JS, no build step)
- `assets/` — app icons used on the cards
- `.nojekyll` — serve files as-is on GitHub Pages

## Apps & links
Listed in card order.

| App | Page (GitHub Pages) | App Store |
|-----|---------------------|-----------|
| ふぅふぅ       | https://hideto0926.github.io/fufu/           | — (coming soon) |
| ScrollAlbum   | https://hideto0926.github.io/scrollAlbum/    | — (coming soon) |
| 好きぴエール   | https://hideto0926.github.io/cheerNotice/    | https://apps.apple.com/jp/app/%E5%A5%BD%E3%81%8D%E3%81%B4%E3%82%A8%E3%83%BC%E3%83%AB/id6791305109 |
| POLACAM       | https://hideto0926.github.io/PolaCamera/     | https://apps.apple.com/jp/app/polacamera/id6790100189 |
| LoveTypeViewer| https://hideto0926.github.io/LoveTypeViewer/ | https://apps.apple.com/jp/app/lovetypeviewer/id6789917188 |
| Magic Album   | https://hideto0926.github.io/MagicAlbum/     | — (coming soon) |
| instaFolder   | https://hideto0926.github.io/instaFolder/    | https://apps.apple.com/jp/app/instafolder/id6787540013 |
| Rain Cam      | https://hideto0926.github.io/RainDropCam/    | https://apps.apple.com/jp/app/rain-drop-cam/id6785505204 |
| superMosaic   | https://hideto0926.github.io/superMosaic/    | https://apps.apple.com/jp/app/supermosaic/id6778454220 |
| BeatShuffle   | https://hideto0926.github.io/BeatShuffle/    | https://apps.apple.com/jp/app/beatshuffle/id6778877123 |
| BarcodeClip   | https://hideto0926.github.io/barcodeClip/    | https://apps.apple.com/jp/app/barcodeclip/id6782431475 |
| 麻雀EYE        | https://hideto0926.github.io/MahjongEye/     | https://apps.apple.com/jp/app/%E9%BA%BB%E9%9B%80eye/id6784469742 |
| 30minTimer    | https://hideto0926.github.io/30minTimer/     | https://apps.apple.com/jp/app/30mintimer/id6780185941 |

Source pages live in each app's own repo — ふぅふぅ's is `app_fufu/web/`
(not yet pushed to the `fufu` repo, so the card link 404s until it is).

## Deploy (GitHub Pages)
1. Push the contents of this folder to the **root** of the `hpTop` repo
   (https://github.com/hideto0926/hpTop), default branch.
2. Repo → Settings → Pages → Source: *Deploy from a branch* → branch = default, folder = `/ (root)`.
3. Wait ~1 min, then open https://hideto0926.github.io/hpTop/.

## Notes
- Adding a new app: copy a `<article class="card">` block in `index.html`, drop its
  icon in `assets/`, and update the link. Use `badge live` for App Store apps,
  `badge soon` for ones coming soon (page only, no store button yet),
  `badge web` for web-only apps.
- Language defaults to the visitor's browser language and can be toggled top-right;
  the choice is remembered via `localStorage`.
