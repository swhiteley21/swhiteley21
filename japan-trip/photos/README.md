# Photos

Drop your trip photos into this folder to make them appear in the journal,
the hero and the photo wall. Match the filename shown below; the page tries
`.jpg`, `.jpeg`, `.png` and `.webp` automatically, so the name is all that
matters.

The **Add your photos** button on the wall also loads photos straight from your
device for a quick look, but those are not saved, so committing files here is
the way to keep them.

## 1. Hero (the big opening image)

- `hero` — a strong, wide landscape shot for the title screen. Something
  atmospheric: a Tokyo street at night, a torii gate, a temple, the group.
  The page darkens it automatically so the title stays readable.

## 2. The journal (one to three per day)

Tokyo (15–19 May)
- `t01a` `t01b` `t01c` — 7-Eleven egg sando · Shibuya crossing · Asakusa market
- `t02a` `t02b` — Meiji shrine · the first stamp
- `t03a` `t03b` `t03c` — Imperial Palace · Mt Fuji artwork · matcha ice cream
- `t04a` `t04b` — Mt Fuji · forest temple
- `t05a` `t05b` `t05c` — Shibuya Sky · Tsukiji tuna · family izakaya

Kyoto (20–23 May)
- `k06a` `k06b` — Shinkansen · geisha sighting
- `k07a` `k07b` `k07c` — Kinkaku-ji · Kiyomizu-dera · £7.50 sushi
- `k08a` `k08b` — tea ceremony · Nishiki market

Osaka (23–25 May)
- `o09a` `o09b` — Dotonbori · karaoke
- `o10a` `o10b` `o10c` — Hiroshima · okonomiyaki · wagyu feast
- `o11a` `o11b` `o11c` — Nakazakicho · Osaka Castle · matcha frappe

Tokyo again (26–28 May)
- `t12a` — Tokyo return
- `t13a` `t13b` `t13c` — espresso tonic · Yanaka · Hoppy Street
- `t14a` `t14b` — Senso-ji · Nakameguro river

## 3. The photo wall (twelve best-of shots)

- `wall-01` — the eight of us
- `wall-02` — Tokyo neon at night
- `wall-03` — a torii gate
- `wall-04` — best bowl of ramen
- `wall-05` — the stamp book, open
- `wall-06` — Shinkansen on the platform
- `wall-07` — a Kyoto backstreet
- `wall-08` — Mt Fuji
- `wall-09` — a proper matcha
- `wall-10` — Dotonbori lights
- `wall-11` — a market stall
- `wall-12` — a favourite candid

Example: save your Shibuya crossing photo as `t01b.jpg`, your title shot as
`hero.jpg`, and a group photo as `wall-01.jpg`.

## Viewing the page

Open `../index.html` in a browser. Photos load most reliably over HTTP, so from
the `japan-trip` folder you can run `python3 -m http.server` and visit
`http://localhost:8000`.
