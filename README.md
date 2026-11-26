# Front page: the world news of Thursday 26 November 2026

[![make.fun · news-image-20261126](https://make.fun/badge/news-image-20261126.svg)](https://make.fun/bounty/news-image-20261126?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)
[![rank](https://make.fun/badge/news-image-20261126/FajarRizikAinulyakin/makefun-news-image-20261126/rank.svg)](https://make.fun/bounty/news-image-20261126/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)
[![reward](https://make.fun/badge/news-image-20261126/FajarRizikAinulyakin/makefun-news-image-20261126/reward.svg)](https://make.fun/bounty/news-image-20261126?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)

This repository holds a single image: a 1024 by 1024 newspaper front
page for Thursday 26 November 2026, published under the MIT license.

The front page, "THE WORLD TODAY", sums up the day's world news:

- **Lead:** Trump unveiled new tariffs on 14 trading partners — up to
  20% on Chinese goods, 15% on the EU, Japan and South Korea — in a
  bid to counter subsidised overcapacity (Reuters).
- **Ukraine war:** Kyiv said it damaged five Russian jets — three
  MiG-31s and two Su-34s — at Savasleyka air base, and hit two
  Rosneft refineries in Samara (Reuters, BBC).
- **Oil:** the Houthis claimed a strike on Saudi Arabia's Ras Tanura
  refinery and Riyadh's financial district; Brent crude settled 3.5%
  higher at $94.61 a barrel (Reuters).
- **Sudan:** RSF drone strikes killed 19 civilians, including six
  women, in Damazin, Blue Nile state (Reuters).
- **The cost of war:** leaked Rosstat figures analysed by the BBC put
  Russian military deaths in Ukraine at at least 490,334 since
  February 2022.
- **Egypt:** a fuel truck overturned and caught fire on Greater
  Cairo's Ring Road, killing at least 30 people (Reuters).

In brief: Norway's top court ruled climate-disputed oil licences
invalid; Colombian police freed 20 supermarket hostages after 17
hours; China welcomed the first Pakistani astronaut aboard its
Tiangong station; Kenya discharged its last Ebola patient as the DRC
death toll passed 5,300.

## The program

`main.py` is a standard-library-only Python program. Run it and it
draws the front page from scratch — text with a built-in 5x7 bitmap
font, rules and panels on a raster canvas, encoded as a PNG with
`zlib` and `struct` — and writes it to the output directory
(`$MAKEFUN_OUTPUT_DIR`, or `/output` by default). It takes no
arguments, uses no network, and produces identical bytes on every
run; the output is checked against the SHA-256 digest recorded in
the program.

## Files

- `entry.png` — the 1024 by 1024 front page (22,455 bytes)
- `main.py` — the drawing program
- `LICENSE` — MIT license
