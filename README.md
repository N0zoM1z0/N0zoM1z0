<div align="center">

<a href="https://n0zom1z0.github.io/touhou-university/">
  <img src="https://raw.githubusercontent.com/N0zoM1z0/touhou-university/main/assets/crest.svg" width="80" alt="TouHou University crest">
</a>

# Hi, I'm N0zoM1z0 👋

### Senior Incident Resolver @ [TouHou University](https://n0zom1z0.github.io/touhou-university/)

**Reverse engineering · game systems · music tooling · formal methods · zero-knowledge systems**

</div>

My GitHub is what happens when a Touhou fan treats curiosity as an incident-response process. This has caused several incidents.

The name `N0zoM1z0` is **Nozomi + Mizore**, from [*Liz and the Blue Bird*](https://liz-bluebird.com/)—my favorite film from the *Sound! Euphonium* series—with just enough leetspeak to become an internet handle. That probably explains why music keeps sneaking into my engineering projects.

I reconstruct old games from binaries, build agents that dodge danmaku through the games' real input paths, turn private replays into zkVM witnesses, and occasionally ask coding agents to make IA sing. Formal methods stop the fun from quietly turning into a false claim.

## 📖 Field Notes from Beyond the Barrier

The code lives here. On my **[personal site](https://n0zom1z0.github.io/)**, I write about how I got there: which assumptions failed, which experiments went nowhere, what finally worked, and what I still can't prove.

The front door has a small spin-to-reveal ritual—because even the blog has a spell-card gate.

**[Cross the Barrier → read the field notes](https://n0zom1z0.github.io/)**

## ⛩️ Department of Danmaku Engineering

Most of my office hours are spent investigating incidents in Gensokyo.

- **Source reconstruction** — rebuilding [TH07](https://github.com/N0zoM1z0/th07), [TH08](https://github.com/N0zoM1z0/th08), and [TH10.5](https://github.com/N0zoM1z0/th105) against their original Japanese executables. “Looks equivalent” does not count. The bytes have veto power.
- **Reverse engineering with receipts** — build-specific address maps, runtime experiments, and byte-checked patches for [Imperishable Night and Scarlet Weather Rhapsody](https://github.com/N0zoM1z0/touhou-reverse-engineering).
- **The game is the oracle** — the [TH06](https://github.com/N0zoM1z0/touhou-solver-th06), [TH08](https://github.com/N0zoM1z0/touhou-solver-th08), and [TH10.5](https://github.com/N0zoM1z0/touhou-solver-th105) agents read native state and send controlled input back to pinned retail builds. Each game gets a different mix of route planning, differential experiments, and bounded learning; the retail game gets the final say.
- **Faster and stranger Gensokyo** — a deterministic, accelerated [Linux TH06 runtime](https://github.com/N0zoM1z0/th06-headless) for solver/RL research, plus [zkTH06](https://github.com/N0zoM1z0/zkTH06): replay-verified Touhou semantics, gradually smuggled into OpenVM. Apparently Gensokyo has a proving system now.
- **The actual university** — the joke got out of hand, so [幻想鄉立東方大學](https://n0zom1z0.github.io/touhou-university/) now has a trilingual campus, research ethics, incident dossiers, and a suspicious amount of lunar paperwork.

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

My professional focus is **formal methods and zero-knowledge systems**. I care about program semantics, translation validation, SMT/CEGIS, and verifiable execution—especially the gap between “the proof checked” and “we proved the right thing.”

- **[VeriMorph](https://github.com/N0zoM1z0/verimorph)** tests low-level transformations against explicit semantics and side conditions, with a fully specified small VM and a deliberately narrow x86-64 ELF target.
- **[Sphinx Interrogator](https://github.com/N0zoM1z0/sphinx-interrogator)** uses relational observations, automata learning, and SMT/CEGIS to recover hidden state from a deliberately leaky microcoded VM.
- **[zkTH06](https://github.com/N0zoM1z0/zkTH06)** is the crossover episode: recover retail Touhou gameplay semantics frame by frame, then make a private replay the witness to an OpenVM proof.
- **[ProofMark](https://github.com/N0zoM1z0/ProofMark)** combines anonymous eligibility, blind marking, tamper-evident logs, and Noir proofs in a privacy-preserving assessment workflow.

## 🌏 Appointments in the Outside World

TouHou University approved my outside-world paperwork. Somehow. Beyond the Barrier, I work with:

- **[Preference Labs](https://x.com/preftrade)** — with [morluto](https://github.com/morluto/), I work on [Jacobian](https://github.com/morluto/jacobian) for exact mathematics and independent checking, [LeanToken](https://github.com/morluto/leantoken) for finding the code that matters, and [Preference](https://preference.net/) for reasoning over prediction markets and world signals. Three ways of asking an agent to please look at the evidence before sounding confident.
- **[Bera Buddies](https://github.com/berabuddies/)** — I'm a research intern working on zero knowledge, formal methods, and agent security. Most of it is still private; the Barrier is doing its job :3

## 🎧 After Office Hours

On matters no proof system can settle, I maintain aggressively non-neutral priors:

- 🌿 **Visual novel:** Key's [*Rewrite*](https://key.visualarts.gr.jp/rewrite/index2.html). No counterexample accepted.
- 🕊️ **Liz:** the complete 47-track [*Liz and the Blue Bird*](https://liz-bluebird.com/) soundtrack, kept in DSF. Some feelings require DSD.
- 🌕 **Lunar allegiance:** TH08 → Eientei → Kaguya → “竹取飛翔 ～ Lunatic Princess.” Absolute single-target routing; Eirin handles incident response: `(ﾟ∀ﾟ)o彡゜えーりん！えーりん！` My music folder turns up roughly thirty related files. This is no longer a preference; it is a replication study. The one I keep returning to is nmk's [“sola”](https://booth.pm/ja/items/3195221) from *千紫万紅* (`MMO-12`, Reitaisai 9, 2012-05-27).
- 🎤 **VOCALOID:** IA is my favorite voicebank; Natsume Chiaki's Miku track [“花色日和”](https://www.youtube.com/watch?v=4rDdRVm3q8U) from *天響ノ和樂2* is my favorite song. Favorite voice and favorite song are separate variables. Q.E.D. ...probably.

## 📟 Gensokyo Incident Board

| Incident | Official response |
| --- | --- |
| `th08.exe` refuses to explain itself | Open IDA. Follow the state write. Bring receipts. |
| A Touhou solver clears only in simulation | Return it to the retail game. No shrine credit yet. |
| Another “Lunatic Princess” arrangement appears | Archive it immediately. Current count: ≈30. Severity: critical. |
| A private TH06 replay requests proof of existence | Put Gensokyo in OpenVM. What could possibly go wrong? |
| University paperwork is missing a lunar seal | Escalate to Eientei. Expected response time: **永遠**. |

<div align="center">

**Currently on call for danmaku incidents, lunar paperwork, singing robots, and theorems that looked much better before someone wrote down the statement.**

</div>
