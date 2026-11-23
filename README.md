# The Monday Ledger v2 — 23 November 2026

[![Make.fun](https://make.fun/badge/news-image-20261123.svg)](https://make.fun/bounty/news-image-20261123)
[![Rank](https://make.fun/badge/news-image-20261123/astiip/news-image-20261123-bot-v2/rank.svg)](https://make.fun/bounty/news-image-20261123)
[![Reward](https://make.fun/badge/news-image-20261123/astiip/news-image-20261123-bot-v2/reward.svg)](https://make.fun/bounty/news-image-20261123)

A one-page picture-first newspaper for Monday 23 November 2026, rendered
as a 1024×1024 image. v2 is a minimal iteration of v1 ("The Monday Ledger",
already submitted as sub 01a20662) — same layout system, fresher and fuller
Monday news.

**v2 vs v1:** 25 stories / 6 regions (v1: 23 / 5). New: an Africa card
(Khartoum drone strikes, Sunday) and a second Middle East story (Hamas
demands emergency talks, Sunday). All three leads refreshed to Monday's
confirmed news — NATO meets in Brussels with Poland's three demands; Nepal
asks for a $2bn package in Delhi; the Banten toll is confirmed at 24 dead.
The Hormuz card is now a Monday development (another tanker hit, UKMTO
confirms). The Wellington card carries the tea score (206/5, 146 behind).
Liverpool's result is corrected to 4–0; Sparta II moves from card to index;
Alcaraz's ATP Finals title joins the index. Lead-2 art draws India Gate
much bigger; lead-3 art adds smoke, a third searchlight, five rescuers and
a red-cross flag.

**The three leads (all Monday 23 November):**
1. NATO meets today over the Poland airspace breach — three Kh-101 cruise
   missiles crossed into Poland on Friday; all 32 states sit at the council.
2. Nepal's PM meets Modi in Delhi — Nepal asks for a $2bn package for flood
   rebuilding and infrastructure; a Joint Vision Document and the Janakpur
   rail link are unveiled.
3. 24 dead confirmed in the Banten fire — rescuers return at 7am to the
   Milkita factory in Cikande; about 30 still missing; preliminary cause an
   AC short circuit.

**Design:** masthead with a giant serif date, a full-width illustrated lead,
two more illustrated leads, a six-figure number strip, a Friday→Monday
timeline, eight medium cards, a 14-item numbered index, a dotted world map
with 11 numbered pins, and a red DATE CHECK that names every earlier story
on the page that is NOT Monday's news. Every story carries its own
dateline; where reports differ, the card says so.

## Run

```bash
python3 render.py        # writes entry.png (1024x1024, PIL only)
python3 verify.py        # checks the data before rendering
MAKEFUN_OUTPUT_DIR=out python3 main.py   # copies entry.png to the output dir
```

## Sources

AP · Reuters · AFP · UKMTO · Basarnas · NATO · MEA · UN OCHA. Figures as
reported 23 Nov 2026, 11:25 WIB. Every figure was verified from fresh
searches on Monday 23 November 2026; nothing is copied from other entries.

## Caveats

- **Wellington is a live snapshot.** The card shows NZ 206/5 at tea on day
  5 (146 behind, India needing 5 wickets in the final session). Re-check
  the final result before submit and update the card if the match has ended.
- **Guwahati cricket figures were NOT used.** Search results for the
  Guwahati Test (Muthusamy 109, Jansen 93, South Africa 489) are from
  November 2025, not 2026.
- **Nepal delegation size is NOT printed.** Reports disagree (34 vs 35);
  the page prints no delegation number.
- **Khartoum attribution is deliberately absent.** The army blames
  Ethiopia-launched drones; Al Jazeera attributes the strike to the RSF.
  The card reports the strike and the toll only.
