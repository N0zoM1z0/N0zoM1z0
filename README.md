<div align="center">

<a href="https://n0zom1z0.github.io/touhou-university/">
  <img src="https://raw.githubusercontent.com/N0zoM1z0/touhou-university/main/assets/crest.svg" width="80" alt="TouHou University crest">
</a>

# Hi, I'm N0zoM1z0 👋

### 🔬 Senior Incident Resolver @ [Touhou-Lab](https://github.com/Touhou-Lab) · ⛩ Founding President of [@Touhou-University](https://n0zom1z0.github.io/touhou-university/) · 🌏 Outside-World Student @ [Tsinghua University](https://www.tsinghua.edu.cn/en/)

**Reverse engineering · game systems · music tooling · formal methods · zero-knowledge systems**

<br>

![Visitors from the Outside World](https://komarev.com/ghpvc/?username=N0zoM1z0&label=Visitors%20from%20the%20Outside%20World&color=blueviolet&abbreviated=true)

</div>

My GitHub is what happens when a Touhou fan treats curiosity as incident response. This has caused several incidents.

The name `N0zoM1z0` is **Nozomi + Mizore**, from [*Liz and the Blue Bird*](https://liz-bluebird.com/), with just enough leetspeak to survive as an internet handle. That probably also explains why music keeps finding its way into repositories that were supposed to be about something else.

I reverse engineer old games, build agents that have to survive the games they claim to understand, and use formal methods whenever “looks right” stops being a useful standard. Sometimes I also ask coding agents to make IA sing.

If a postmortem grows too large for a README, it usually escapes to my **[personal site](https://n0zom1z0.github.io/)**.

## 📟 Gensokyo Incident Board

What I'm working on right now, translated into the University's preferred reporting format.

| Incident | Current response |
| --- | --- |
| `th08.exe` escaped its original habitat | Keep the reconstructed 1.00d code honest, run it natively on Linux, and make the same game logic survive a browser tab: [th08](https://github.com/N0zoM1z0/th08) · [th08-web](https://github.com/N0zoM1z0/th08-web). |
| Danmaku files are far too trusting | [DanmakuFuzz](https://github.com/Touhou-Lab/DanmakuFuzz) mutates ECL, replays, ANM, and retail file formats in fast campaigns, then asks the shipped game under Wine whether the weirdness is real. |
| Lunatic still refuses to clear itself | [TH06](https://github.com/N0zoM1z0/touhou-solver-th06), [TH06 RL](https://github.com/N0zoM1z0/touhou-solver-th06-rl), [TH08](https://github.com/N0zoM1z0/touhou-solver-th08), [TH08 RL](https://github.com/N0zoM1z0/touhou-solver-th08-rl), [TH10.5](https://github.com/N0zoM1z0/touhou-solver-th105), and [PC-98 RL](https://github.com/Touhou-Lab/touhou-pc98-rl) are all variations on the same long-running incident: read the real game, return controlled input, and somehow make the machine learn to dodge the bullets for me. The dream is simple: **Lunatic NMNB, with my hands nowhere near the keyboard.** XD |
| A private TH06 replay says “trust me” | [zkTH06](https://github.com/N0zoM1z0/zkTH06) keeps pulling more of the retail game's frame-by-frame semantics across the proof boundary and into OpenVM. |
| Coding agents all became the same polite intern | [Gensokyo Skills](https://github.com/N0zoM1z0/gensokyo-skills) gives Reimu, Marisa, Yukari, Nitori, and friends genuinely different problem-solving workflows—and evals to catch them if they collapse back into generic advice. |

## ⛩️ Department of Danmaku Engineering

Most of my office hours are still spent investigating incidents in Gensokyo.

The lab rule is simple: **simulation may suggest; the shipped game gets the final say.**

- **Reconstruction with receipts** — [TH07](https://github.com/N0zoM1z0/th07), [TH08](https://github.com/N0zoM1z0/th08), and [TH10.5](https://github.com/N0zoM1z0/th105) are source-reconstruction projects tied back to their original Japanese executables. [Touhou Reverse Engineering](https://github.com/N0zoM1z0/touhou-reverse-engineering) holds the address maps, runtime experiments, patches, and other evidence gathered along the way. “Looks equivalent” is not a matching criterion.

- **Getting old games to run somewhere they were never invited** — the reconstructed TH08 code now has a playable modern Linux path, while [TH08 Web](https://github.com/N0zoM1z0/th08-web) compiles the game logic to WebAssembly and runs entirely in the browser with locally supplied retail DAT files. One endless night, now also a browser problem.

- **Agents that answer to the game** — the TH06, TH08, and TH10.5 solvers each use a different mix of state extraction, planning, experiments, and learning, but they share one contract: observe the real game, act through controlled input, and do not award shrine credit for a route that only works in a convenient model. The newer [TH06 RL](https://github.com/N0zoM1z0/touhou-solver-th06-rl), [TH08 RL](https://github.com/N0zoM1z0/touhou-solver-th08-rl), and [PC-98 RL](https://github.com/Touhou-Lab/touhou-pc98-rl) experiments keep learning behind explicit safety and evidence boundaries.

- **Fuzzing the spell machinery** — [DanmakuFuzz](https://github.com/Touhou-Lab/DanmakuFuzz) treats ECL timelines, replay payloads, ANM resources, and game file formats as structured mutation targets. Headless execution is the fast scout; reduction makes the result understandable; Wine and the retail game decide whether a finding gets promoted.

- **Faster Gensokyo, with disclaimers** — [th06-headless](https://github.com/N0zoM1z0/th06-headless) strips TH06 down to a deterministic accelerated Linux logic runtime for solver, replay, and RL research. It is useful for generating evidence quickly. It is deliberately not allowed to appoint itself the oracle.

- **Proof-carrying spell cards** — [zkTH06](https://github.com/N0zoM1z0/zkTH06) starts from differential traces against the shipped game, rebuilds gameplay semantics a boundary at a time, and feeds private replay input into OpenVM proofs. Apparently “did this run really happen?” is now a zero-knowledge question.

## 🎛️ Department of Synthetic Voices & Hit Circles

- **[VOCALOID MCP](https://github.com/N0zoM1z0/vocaloid-mcp)** — an MCP server that lets coding agents compose, tune, render, mix, and audit native VOCALOID3/4 projects. It can validate the project and its native rendering path. It cannot prove that the song is good; human listening retains jurisdiction.
- **[osu! Reverse Engineering](https://github.com/N0zoM1z0/osu-reverse-engineering)** — native parsers, planners, and in-process timing experiments for mania, taiko, and catch, plus a static analysis of the client's integrity mechanisms.

*Catch autoplay field report: **99.93%, 2,806pp** on Flowering Night Fever. osu! later banned the account—fair enough, honestly XD. The experiment is over; the screenshot survives.*

<p align="center">
  <a href="https://github.com/N0zoM1z0/osu-reverse-engineering/tree/main/catch">
    <img src="./assets/osu-catch-2806pp.png" width="1000" alt="osu!catch autoplay result on Flowering Night Fever: 99.93% accuracy and 2,806pp">
  </a>
</p>

- **[oszillator](https://github.com/N0zoM1z0/oszillator)** — drop an `.osz` into the browser and play. Web Audio owns the clock; Pixi owns the playfield; your beatmap never leaves your machine. [Try the live demo →](https://n0zom1z0.github.io/oszillator/)

## ∀ Department of Things That Should Actually Be True

I spend a lot of time on programs that are supposed to justify themselves.

The recurring question is not just “did the checker accept it?” but **what exactly did we model, and is that actually the thing we meant to claim?**

- **[VeriMorph](https://github.com/N0zoM1z0/verimorph)** — low-level program transformations with explicit semantics, checked side conditions, synthesis where search is actually useful, and translation validation before transformed bytes are allowed out. The x86-64 path stays narrow on purpose: unsupported cases are much better than quietly invented guarantees.

- **[Sphinx Interrogator](https://github.com/N0zoM1z0/sphinx-interrogator)** — a deliberately leaky microcoded VM and a black-box interrogator trying to recover its hidden state. Instead of brute-forcing one noisy signal, it designs relational experiments, learns the hidden machine, and uses SMT/CEGIS to decide what question is worth asking next.

- **[zkTH06](https://github.com/N0zoM1z0/zkTH06)** — the inevitable Touhou crossover episode. Start with frame-by-frame evidence from the retail game, make the executable semantics precise enough to reproduce, then ask a private replay to carry the witness through OpenVM. The proof is only as interesting as the boundary it actually covers.

- **[ProofMark](https://github.com/N0zoM1z0/ProofMark)** — a privacy-preserving assessment workflow built around anonymous eligibility, blind marking, tamper-evident records, and Noir proofs. The point is not to put a gradebook on-chain; it is to prove the useful facts without exposing everything else.

## 🌏 Appointments in the Outside World

TouHou University approved my outside-world paperwork. Somehow.

Current postings include:

- **[Tsinghua University](https://www.tsinghua.edu.cn/en/)** — my current outside-world posting. I study how to find holes in the Great Hakurei Barrier, how to tell when something crossed it that should not have, and how to keep Gensokyo on the correct side of the boundary. Sometimes the incident report gets reformatted and submitted in the local academic format known as a *paper*.

- **[Preference Labs](https://x.com/preftrade)** — with [morluto](https://github.com/morluto/), I work on [Jacobian](https://github.com/morluto/jacobian), [LeanToken](https://github.com/morluto/leantoken), and [Preference](https://preference.net/): exact mathematics, finding the code that matters, and getting agents to look at the evidence before they commit to a story.

- **[Bera Buddies](https://github.com/berabuddies/)** — I'm a research intern working on zero knowledge, formal methods, and agent security. Most of the interesting work is still private; the Barrier is functioning as designed :3

## 🎧 After Office Hours

When the work stops, the methodology becomes considerably less rigorous.

- 🌿 **Visual novel:** Key's [*Rewrite*](https://key.visualarts.gr.jp/rewrite/index2.html). Favorite means favorite. I am not accepting review comments on this one.

- 🕊️ **Liz:** I keep the complete 47-track [*Liz and the Blue Bird*](https://liz-bluebird.com/) soundtrack in DSF. Is that necessary? No. Is it staying that way? Absolutely.

- 🌕 **Lunar allegiance:** TH08 → Eientei → Kaguya → “竹取飛翔 ～ Lunatic Princess.” Eirin still handles incident response: `(ﾟ∀ﾟ)o彡゜えーりん！えーりん！` My music folder contains roughly thirty related files, which is probably enough evidence to stop calling this a casual preference. The arrangement I keep coming back to is nmk's [“sola”](https://booth.pm/ja/items/3195221) from *千紫万紅* (`MMO-12`, Reitaisai 9, 2012-05-27).

- 🎤 **VOCALOID:** IA is my favorite voicebank; Natsume Chiaki's Miku track [“花色日和”](https://www.youtube.com/watch?v=4rDdRVm3q8U) from *天響ノ和樂2* is my favorite song. Favorite voice and favorite song are separate variables. Q.E.D. ...probably.

<div align="center">

**Currently on call for danmaku incidents, lunar paperwork, singing robots, and theorems that looked much better before someone wrote down the statement.**

</div>
