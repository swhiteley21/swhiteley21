# Photos

Drop your trip photos into this folder to make them appear permanently in the
journal. Each photo slot on the page shows the filename it is looking for, and
the page tries `.jpg`, `.jpeg`, `.png` and `.webp` automatically, so you only
need to match the name.

You can also use the **Add your photos** button in The Wall section to load
photos straight from your device for viewing. Those stay on your screen only
and are not saved, so the folder below is the way to keep them.

## Filenames the journal looks for

Tokyo (15–19 May)
- `t01a` `t01b` `t01c` — egg sando, Shibuya crossing, Asakusa market
- `t02a` `t02b` — Meiji shrine, the first stamp
- `t03a` `t03b` `t03c` — Imperial Palace, Mt Fuji artwork, matcha ice cream
- `t04a` `t04b` — Mt Fuji, forest temple
- `t05a` `t05b` `t05c` — Shibuya Sky, Tsukiji tuna, family izakaya

Kyoto (20–23 May)
- `k06a` `k06b` — Shinkansen, geisha sighting
- `k07a` `k07b` `k07c` — Kinkaku-ji, Kiyomizu-dera, £7.50 sushi
- `k08a` `k08b` — tea ceremony, Nishiki market

Osaka (23–25 May)
- `o09a` `o09b` — Dotonbori, karaoke
- `o10a` `o10b` `o10c` — Hiroshima, okonomiyaki, wagyu feast
- `o11a` `o11b` `o11c` — Nakazakicho, Osaka Castle, matcha frappe

Tokyo again (26–28 May)
- `t12a` — Tokyo return
- `t13a` `t13b` `t13c` — espresso tonic, Yanaka, Hoppy Street
- `t14a` `t14b` — Senso-ji, Nakameguro river

Example: save your Shibuya crossing photo as `t01b.jpg` in this folder.

## Viewing the page

Open `../index.html` in a browser. Photos load best when served over HTTP, so
from the `japan-trip` folder you can run `python3 -m http.server` and visit
`http://localhost:8000`.
