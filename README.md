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
| Mercury       | https://hideto0926.github.io/mercuryGame/    | — (coming soon) |
| 音の神経衰弱   | https://hideto0926.github.io/musicGame/      | — (coming soon) |
| ドンピタ｜花火の音ズレ補正 | https://hideto0926.github.io/hanabi/ | https://apps.apple.com/jp/app/%E3%83%89%E3%83%B3%E3%83%94%E3%82%BF-%E8%8A%B1%E7%81%AB%E3%81%AE%E9%9F%B3%E3%82%BA%E3%83%AC%E8%A3%9C%E6%AD%A3/id6804727858 |
| かみバトル     | https://hideto0926.github.io/kamiBattle/     | https://apps.apple.com/jp/app/kamibattle/id6801514915 |
| SHIBA TOWER   | https://hideto0926.github.io/shibaTower/     | https://apps.apple.com/jp/app/shiba-tower/id6800798024 |
| ふぅふぅ       | https://hideto0926.github.io/fufu/           | https://apps.apple.com/jp/app/%E3%81%B5%E3%81%85%E3%81%B5%E3%81%85-%E6%81%AF%E3%81%A7%E3%81%86%E3%81%8B%E3%81%9B%E3%82%8B%E9%A2%A8%E8%88%B9%E3%82%B2%E3%83%BC%E3%83%A0/id6797118306 |
| ScrollAlbum   | https://hideto0926.github.io/scrollAlbum/    | https://apps.apple.com/jp/app/scrollalbum/id6793163045 |
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

Source pages live in each app's own repo.

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
- The three.js background builds its flying icons from every card's `.icon` image,
  so a new card's icon shows up there automatically.
- Language defaults to the visitor's browser language and can be toggled top-right;
  the choice is remembered via `localStorage`.
