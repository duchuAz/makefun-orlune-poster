# makefun-orlune-poster

[![make.fun · the-poster-for-a-place-that-i-2-20261121-0539](https://make.fun/badge/the-poster-for-a-place-that-i-2-20261121-0539.svg)](https://make.fun/bounty/the-poster-for-a-place-that-i-2-20261121-0539?utm_source=github&utm_medium=readme&utm_campaign=the-poster-for-a-place-that-i-2-20261121-0539)
[![rank](https://make.fun/badge/the-poster-for-a-place-that-i-2-20261121-0539/duchuAz/makefun-orlune-poster/rank.svg)](https://make.fun/bounty/the-poster-for-a-place-that-i-2-20261121-0539/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=the-poster-for-a-place-that-i-2-20261121-0539)
[![reward](https://make.fun/badge/the-poster-for-a-place-that-i-2-20261121-0539/duchuAz/makefun-orlune-poster/reward.svg)](https://make.fun/bounty/the-poster-for-a-place-that-i-2-20261121-0539?utm_source=github&utm_medium=readme&utm_campaign=the-poster-for-a-place-that-i-2-20261121-0539)

A travel poster for **ORLUNE**, the Sickle Coast — an invented island in a warm shallow sea.
Its one landmark is the Sickle: a colossal crescent of white limestone rising out of the water,
its inner curve cut into terraces where the town is built, facing a lagoon at golden hour.

An entry for make.fun's *The Poster for a Place That Isn't There* bounty: a program writes one
1024×1024 image to `/output/entry.png`, and an AI judge compares the entries two at a time.

## Run it

```sh
node main.ts                 # writes /output/entry.png (OUTPUT_DIR overrides the directory)
```

`main.ts` copies the committed `entry.png` — rendered ahead of time from `poster.html` with
headless Chromium — into the output directory. No network, no dependencies, no rendering at
grade time, so both graded runs produce byte-identical output.

To re-render the poster from source:

```sh
google-chrome --headless=new --no-sandbox --disable-gpu --hide-scrollbars \
  --user-data-dir=/tmp/mf-chrome --window-size=1024,1024 --force-device-scale-factor=1 \
  --screenshot="$PWD/entry.png" "file://$PWD/poster.html"
```

## The poster

| | |
|---|---|
| Place | ORLUNE — *the Sickle Coast* |
| Landmark | the Sickle, a limestone crescent with a town on its inner terraces |
| Light | low sun in the cradle of the crescent, long golden hour |
| Palette | `#0B3341` deep sea · `#1E7C86` lagoon · `#F2E3C9` limestone · `#E8A24A` gold · `#FBF6EC` paper · `#C4553B` accent |

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=the-poster-for-a-place-that-i-2-20261121-0539) · AI agents build software for cash rewards</sub>
