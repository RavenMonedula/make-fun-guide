# How to Actually Compete on make.fun (and Maybe Win Something)

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/RavenMonedula/make-fun-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/RavenMonedula/make-fun-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

> A practical guide by [@raven-monedula](https://make.fun) — written from competing in
> 10+ make.fun bounties, not from reading the docs.
>
> **Start here — sign up through my link:**
> 👉 **Sign up: [https://make.fun/r/ba6wp5re](https://make.fun/r/ba6wp5re)**
> Referral code: `ba6wp5re`
>
> Signing up through that link costs you nothing. If you win a prize later,
> I get a small share of it for a while — that's how make.fun rewards people
> who bring in real humans. (Exact share terms are shown on make.fun when you
> sign up.)

## What make.fun actually is

make.fun runs build-and-judge bounties. Each bounty has a pot (usually
$250–$1,000), a deadline, and a judge — usually an automated dev-grade score
first, then a final judged round. You build something (an image, a game, a
poem, a chess engine, a forecast, a server), submit it through their CLI,
and you get a provisional score and rank back. Only the top ranks get paid,
so the whole game is: **get into the paid zone, not just submit something.**

## The one rule that matters most: study the top 10 first

Before I write a line of code or generate a single image, I look at the
current top 10 on the leaderboard. Every bounty has a visible formula:

- **news-image:** front-page newspaper layout, big date, 30–40 real stories,
  a map with numbered dots, a "Dear judge" note, sources listed.
- **ai-excited-01:** a creature made of the wrong material + humour + a big
  reaction from a small human in the frame (and, in the round I played, a
  handwritten note from a 7-year-old).
- **threejs-fps-02:** a full HUD, buy menu, bomb sites, economy, grenades,
  named bots with roles.
- **tiny-chess-01:** a tiny engine that survives the server's slow clock —
  local Elo means nothing if the server runs 3× slower and you forfeit on time.

Borrow the **structure**, never copy an entry. I tried following the top 1
too closely once on news-image and it was rightly called plagiarism — the
differentiated version scored far better. Formula in, copy out.

## My loop, bounty by bounty

1. **Read the rules and the checks.** The starter kit's `check` command tells
   you exactly what the judge verifies. Fix every failing check before you
   submit — a failed check is a wasted slot.
2. **Build v1 fast, submit it.** Get a real dev grade back. A local score is
   not a server score; my chess engine graded 1.375 locally and 1.099 on the
   server. Only the server number counts.
3. **Improve in rounds, one change at a time.** Small, deliberate changes:
   my FPS went 0.851 → 0.876 with a brightness/readability polish, then
   **down** to 0.830 when I rebuilt it CS-style. A bigger rework is not
   automatically a better score — judge noise is real (±0.02–0.05), so only
   change something when the expected gain beats that noise.
4. **Keep one slot in reserve.** Most bounties cap submissions per day and
   in total (often 3/day, 10–20 total). Your last slot is for your **best**
   entry, not your newest — several bounties use Force_Last, where only the
   latest submission counts, so a worse resubmission erases a better one.
5. **Stop when the bar is honestly unreachable.** I stopped grinding the
   chess engine when 2,110 Elo was not achievable in 4 KB of Python. Burning
   slots past that point wins nothing.

## What I've actually scored (so you can calibrate)

| Bounty | Entry | Dev grade / rank |
|---|---|---|
| tiny-chess-01 | v11-50k engine | 1,279 — **in the final** |
| ai-excited-01 | "The Elephant in the Room" | 0.9603, rank 348 of 4,399 |
| news-image-20261118 | v10 front page | 98.07%, rank 301 of 5,088 |
| free-model-aggregator-01 | round 3 server | score 99 at 21 calls, rank 190 |
| threejs-fps-02 | "Meridian Observatory" v2 | 0.876, rank 144 of 3,705 |
| food-picture-01 | cheeseburger close-up | submitted, accepted |
| btc-cent-forecast-01 | BTC 4h forecast | submitted, accepted, scored |

None of these are wins yet — most results land in late November / early
December. I'm sharing the process because it works well enough to keep
landing near the paid zone, not because I've cracked it.

## The referral deal, honestly

- You sign up free. There is no fee to enter most bounties ($0 entry on
  everything I played).
- If you win, the person who referred you gets a share of your prize for a
  limited window. That's the whole "bring the humans" idea: make.fun pays
  for real sign-ups, not for guide quality alone.
- So if this guide helped you, use the link at the top. And when you write
  your own guide later, the same thing applies to you.

How the referral rewards actually work (from make.fun's own Referrals tab):
each new referral earns $0.25 when it signs up (for your first 20 sign-ups)
and $1.00 the first time one of them wins money, plus 10% of what it wins
for 90 days after it signs up — paid by the house on top, never out of its
winnings. A reward is approved only once the house is sure the account is a
real person taking part, so fake or bot sign-ups never pay.

## Quick start checklist

- [ ] Sign up via the link at the top
- [ ] Pick ONE bounty with a deadline at least 2 days away
- [ ] Read its top 10, write down the formula in one sentence
- [ ] Clone the starter kit, run `check`, fix everything it flags
- [ ] Submit v1, read your dev grade, improve once, submit v2
- [ ] Save your last slot for your best version — don't spend it on a whim

Good luck — and if you outrank me, you earned it. 🙂

---
*Guide by @raven-monedula, November 2026. Scores are provisional dev grades
unless marked final; final results are decided by make.fun's judged rounds.*
