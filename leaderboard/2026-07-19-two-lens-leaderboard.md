# Two-lens model leaderboard — first results, and please tear it apart

**Status: methodology hypothesis, actively inviting red-team.** These are early numbers on a small set; the point of posting is to be attacked, not believed.

We scored current models on **code-review discrimination** (can a model tell buggy code from clean, with calibrated confidence?) — Brier-scored against known ground truth. We rank it **two ways**:

- **Performance** (money no object, by calibration): `glm-5.2`, `grok-4`, `grok-3`, `claude-haiku` lead.
- **Value** (a 55/20/25 accuracy·speed·cost composite): the **free** `llama-3.3-70b` comes first.

The finding we're comfortable stating: **the most accurate model and the best-value model are not the same, and on this task the accuracy gap between the free and frontier leaders is small.** We are deliberately *not* calling this "AI trustworthiness" — it measures code-review discrimination, one narrow proxy, until we validate it against real-world reliability.

## What's wrong with this (we already know some of it)
- **N is small** — mid-board order is within noise; needs ≥50 items + confidence intervals.
- **The proxy may not predict real trustworthiness** — code-review ≠ security auditing ≠ long-horizon reliability.
- **The cost model is rough** ($/1M estimate; ignores rate-limits, context pricing).
- **Public items invite gaming** — we're moving to a rolling, partially-hidden pool.
- **The composite omits ability + long-context** — the value ranking is conditional on short single-turn review.

## Tear it apart
If the method is flawed, the proxy is meaningless, the cost model is broken, or the items are too easy or too public — **[open an issue](https://github.com/DealAppSeo/trust-commons/issues)** with the specific objection and, ideally, a counter-example or a better item set. We will either fix the board or document why we disagree. Competing methodologies and entirely different designs are first-class here.

*Method is public by design — a leaderboard nobody, including us, can grade their own homework on.*
