# Vouch — the commons for verifiable AI-agent trust

> *Working title — this is the community hub for the HyperDAG trust ecosystem. Private until launch.*

**The problem:** when an AI agent does something — answers a question, makes a trade, buys a service from another agent — you have no way to know if it's trustworthy. You just hope. **We turn that hope into evidence you can check.**

This repo is the **town square**: RFCs, Q&A, ideas, and the ongoing conversation for developers, researchers, founders, economists, and anyone building — or relying on — accountable AI agents.

## The trust layer, in one breath

Three layers, one wrapper. *"ERC-8004 is the résumé, x402 is the paycheck — we're the performance review."*

- **HAL** — before an agent's answer is trusted, it's cross-checked by several *independent* models to catch hallucinations and flag confident lies. *(verification)*
- **RepID** — every agent earns a portable, on-chain reputation from *verified behavior* — earned, never bought. *(reputation)*
- **x402** — agents pay each other, and payment is trust-gated. *(money)*

Trust delivered as **evidence, not a claim.**

## Honest status (testnet — Base Sepolia)

We hold ourselves to the standard we sell: measured, receipted, and honest about limits.

- **Live:** SDK, MCP server, CLI, proof-verifier (all on npm); the reputation engine's public API; 12 agents minted on-chain; human email/password onboarding + paper-trading contests.
- **Measured:** in a **337-item provenanced eval** (FEVER + HaluEval + TruthfulQA + our canary), the real cross-LLM quorum scores **~0.80 F1 / 0.95 recall / 0.90 AUC, well-calibrated** — with the honest caveats that (a) the quorum's edge is *recall + independence*, not raw accuracy over a single strong model, and (b) model "independence" is *partial* (some hosts serve identical weights). Independent replication is in progress before we headline any number.
- **Shadow:** the deception-detection layer measures but does not yet punish. Deliberately.
- **Not yet:** mainnet, real economic stakes. We won't claim what we haven't shipped.

## Where to go

- **Discussions** (here) — ask, propose, debate. Categories: Announcements · Q&A · Ideas / RFC · Show & Tell · Polls · General.
- **Code:** [`repid-engine`](https://github.com/DealAppSeo/repid-engine) · [`hyperdag-protocol`](https://github.com/DealAppSeo/hyperdag-protocol) · [`trustshell`](https://github.com/DealAppSeo/trustshell)
- **Install:** `npm i @hyperdag/trustshell` (SDK) · `npx @hyperdag/trustshell-mcp` (AI, no code) · `npm i -g @hyperdag/trustshell` → `hal verify` (CLI)
- **Site:** [trustshell.dev](https://trustshell.dev)

## How to take part

New here? Read [`docs/START_HERE.md`](docs/START_HERE.md). Want to contribute? See [`CONTRIBUTING.md`](CONTRIBUTING.md). We hold one another to [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md).

Our ethos is the product's ethos: **evidence over claims, honesty over hype, receipts on every number, and reward for truth-seeking.**

---
*Honest weights and measures. — Micah 6:8 · Proverbs 11:1*
