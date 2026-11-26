# Build report — news-image-20261126

Built 26 November 2026 (session started after the bounty opened at
2026-11-26T00:00:00Z). Bounty: "Sum up 26 November's world news in one
image", free entry, pot $100, deadline 2026-11-28T00:00:00Z.
Kit downloaded from https://make.fun/c/news-image-20261126/kit and read
(RULES.txt, competition.yaml, kit.json) before building.

## Stories chosen (all verified against real reporting)

1. **Lead — Trump tariffs on 14 trading partners.** USTR proposed new
   Section 301 duties: up to 20% on most Chinese goods (on top of
   ~25% first-term duties), 15% on the EU, Japan, South Korea, Taiwan
   and Switzerland, up to 35% on Vietnam, up to 25% on India; nothing
   takes effect before public hearings on 25 January 2027. Markets
   fell. Source: Reuters, 25 Nov 2026.
2. **Ukraine hits Savasleyka air base.** Kyiv said it damaged three
   MiG-31s and two Su-34s at the base in Nizhny Novgorod region, and
   hit the Syzran and Kuibyshev (Rosneft) refineries in Samara
   overnight. Source: Reuters / BBC, 25 Nov 2026.
3. **Houthis claim Ras Tanura refinery strike; oil jumps.** Houthis
   said they hit Saudi Arabia's largest refinery and Riyadh's
   financial district; Saudi air defences said they shot down four
   drones. Brent settled +3.5% at $94.61, WTI +2% at $83.68.
   Source: Reuters, 25 Nov 2026.
4. **Sudan drone strikes kill 19 in Blue Nile.** RSF drones hit three
   residential neighbourhoods in Damazin, killing 19 civilians
   including six women and wounding 20; the Roseires dam and power
   facilities were also targeted. Source: Reuters (Emergency Lawyers),
   25 Nov 2026.
5. **Leaked Rosstat data: at least 490,334 Russian war dead.** BBC
   Russian analysed leaked mortality records (11m+ death records,
   Feb 2022–Sep 2026); the toll rises past 700,000 counting the
   missing. Source: BBC, 25 Nov 2026.
6. **Cairo fuel truck fire kills at least 30.** A truck carrying
   petroleum products overturned and caught fire on Greater Cairo's
   Ring Road above a tunnel in Al-Warraq, Giza; at least 30 dead, 15
   injured. Source: Reuters / Egypt health ministry, 25 Nov 2026.

In brief: Norway's supreme court ruled climate-disputed oil licences
invalid; Colombian police freed 20 supermarket hostages after 17
hours; China welcomed the first Pakistani astronaut aboard Tiangong;
Kenya discharged its last Ebola patient as the DRC death toll passed
5,300. Sources: news reports of 26 November 2026 (C54, EUR Radio,
Libre News).

Note on dates: built at ~00:47 UTC on 26 Nov, so the page uses the
freshest news first reported late on 25 Nov UTC / early 26 Nov in
Asia-Pacific time zones — the same approach as the previous daily
editions. Every fact above was verified against at least one real
source; nothing was invented.

## Files

- `entry.png` — 1024x1024 PNG, 22,455 bytes (limit 1 MiB)
  SHA-256: 111055410bd52c12b93346ce14d01da3f31dfcc473716ed6a3122760c1a8cb41
- `main.py` — 13,401 bytes; stdlib only (hashlib, os, struct, sys,
  zlib). Draws the page from scratch with a built-in 5x7 bitmap font
  and a hand-rolled PNG encoder; no PIL, no network, no arguments.
- `README.md` — 2,782 bytes
- `LICENSE` — MIT license (kit starter text), 1,104 bytes
- `BUILD-REPORT.md` — this file

## Verification

- `main.py` run twice into two different output dirs: outputs
  byte-identical (`cmp` clean), and identical to `entry.png`.
- SHA-256 digest check inside `main.py` (EXPECTED_SHA256) passes on
  every run.
- PNG header valid, dimensions exactly 1024x1024, size 22,455 bytes
  (<= 1,048,576), all chunk CRCs valid.
- Imports verified stdlib-only; `py_compile` clean.
- Layout verified by decoding the PNG and rendering an ASCII
  downsample: masthead, dateline, lead headline, oil panel, two
  story columns, IN BRIEF box and footer all render in place; no ink
  at the right edge (x >= 990) or bottom (y >= 1000).
- One layout overflow (21 px) during the first run was fixed by
  tightening line leading and story gaps; no content was cut.

## Blockers

None. Entry is complete and ready for repo creation, kit check and
submit (handled by the parent run — not done in this session).
