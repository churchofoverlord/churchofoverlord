# Church of Overlord — nb-row3 final fix

Cause of the huge vertical gaps:
The deployed `nb-row2.png` was still the original 1536×1024 canvas. The visible parchment occupies only a horizontal strip inside that canvas. The CSS element had the ratio of the cropped version, but `background-size: 100% 100%` was stretching the entire 1536×1024 canvas into it. Result: a very thin visible parchment inside a tall invisible row.

Fix:
- New asset name: `assets/nb-row3.png` (avoids browser/GitHub cache confusion).
- `nb-row3.png` is physically cropped to the parchment itself: 1504×303px.
- CSS aspect ratio exactly matches that file.
- No fixed height.
- Gap between rows is only 8px.
- Old Non-Believers row assets are removed from this package.
- One clean CSS rule set only.

Deploy:
Upload/replace the ENTIRE contents of this ZIP, especially:
- `index.html`
- `assets/nb-row3.png`

The code deliberately uses a NEW filename. Do not rename `nb-row3.png` back to `nb-row2.png`.

After GitHub Pages deploys, Ctrl+F5.
