# UX Research Sprint — Onboarding & Settings IA

**Status:** planning · **Owner:** UX Working Group · **Horizon:** 8–10 week time-boxed sprint · **Last updated:** 2026-06-29

> This is the **operating plan** for the volunteer UX sprint. It is the single
> source of truth for *who is doing what, when, and how*. It is intentionally
> **not** an RFC: RFCs are design *decisions* (the output). This document is the
> research *process* that produces the evidence those decisions need. Findings,
> personas, and synthesis accumulate as sibling files in this `research/` folder.

## What this feeds

Two `proposed` RFCs are explicitly blocked on end-user research — this sprint
unblocks them:

- **RFC 0004 — First-run onboarding** (every frontend ships none today)
- **RFC 0006 — Settings IA & progressive disclosure** (108 params; tier split
  needs empirical validation)

When the research is in, those RFCs are revised to `active` with the evidence
embedded, and engineering implements per platform through the normal RFC
process. **The C API + `settings_manifest.json` remain the cross-platform
parity contract** — UX designs must be expressible through them.

## Prior work (required reading)

This sprint continues, it does not restart. Read first:

- `ux-background/Dasher – settings + onboarding.pdf` — existing IA + onboarding thinking
- `ux-background/Dasher UX milestone 3.pdf` — milestone 3 research output
- Design guide `DESIGN.md` §7 (settings) and §8 (onboarding)
- `governance/rfcs/0004-onboarding.md` and `0006-settings-ia.md`

## Scope

**In:** onboarding (first-run experience) + settings information architecture.
**Out for this sprint:** themes/appearance (RFC 0007 shipped), input-method
redesign, multilingual UI (RFC 0003). Input method enters only *indirectly*,
via persona-branched onboarding.

## Guiding principle: research-led, not solution-led

We do **not** pre-commit to a mechanism. Specifically:

- The current **Game Mode is a hypothesis** for the practice vehicle, not an
  assumption — research may propose something better.
- A **passive "watch how it works" step is a research question**, not a given.
  If one is needed, it's a fresh build or a video clip — `CDemoFilter` was
  removed (`f79eb6a9`) and is **not** to be resurrected.

Engineering choices follow the evidence; they don't lead it.

## Goals & success metrics

"Shorten the gap" means measurably reducing the learning curve for brand-new
users. Lock these before research starts (define baseline, then re-measure):

| Metric | What it tells us |
| --- | --- |
| Time to first correct sentence (novice) | Core first-touch friction |
| Game/practice completion rate, session 1 | Whether the practice loop works |
| Onboarding abandonment % **per step** | The step is the diagnosis |
| % who find a target setting unaided | Settings IA works |
| Params changed by novices | Fewer = better defaults |
| **Retention day 1 / day 7** | The real "did we close the gap" number (needs RFC 0001 analytics) |

## People & roles

Roles are **functions, not people** — several volunteers will likely want to
interview and to prototype, so each can have multiple contributors. Sign-ups
are agreed in the kickoff. All volunteers are contributing in a personal
capacity, independent of any employer.

- **Research lead (volunteer)** — owns research design, ethics/consent, and
  synthesis methodology.
- **Recruit & ops (project lead)** — social-media call, screening survey,
  scheduling, consent, recording storage (align with RFC 0001 privacy stance).
  *This is the project lead's responsibility.*
- **Interviewers / facilitators** (≥1) — run contextual interviews, first-touch
  think-alouds, and usability rounds.
- **Synthesisers** (≥1) — running insights doc; turn recordings into RFC
  evidence.
- **Prototypers** (≥1) — Figma for static flows; web/WASM (real Dasher
  in-browser) for interactive zooming tests; native branch when an input method
  demands it.

Weekly 45-min sync; async channel; hard 8–10 week time-box.

## Recruitment — two cohorts, do not mix

**Existing users cannot answer the onboarding question** — they survived the
learning curve years ago. Segment strictly:

- **Novices (brand-new, never used Dasher)** — for onboarding. Recruited via
  **social media**. Screen for tech-literacy (social respondents self-select
  for it — a known bias); deliberately also recruit lower-tech-literacy users
  via AAC clinics / OTs and switch/eye-gaze device vendors.
- **Existing users (3–4 active panel + wider group)** — for settings IA,
  themes-adjacent, and rapid evaluative rounds.

Personas to cover across both: **mouse / switch / eye-gaze / touch** — they
need different onboarding and different settings defaults.

## Methods, per workstream

- **Settings IA** — async **card sort** (~15–20 from the wider group): users
  group the 108 params themselves, so the basic/advanced/expert split is
  *empirically derived*, not ratifying a maintainer guess. Validate with
  tree-tests ("find 'make Dasher slower'"). Existing-user panel for iteration.
- **Onboarding** — **first-touch think-alouds** with 5 novices on the web/WASM
  build (send a link, screen-share, zero install). The web/WASM build is the
  key enabler for remote novice testing. Switch/eye-gaze persona validation
  happens on native builds with real devices.

Sample sizes are deliberately small-N (5 per usability round, Nielsen) run
frequently — not large-N run once.

## Timeline

| Weeks | Phase | Output |
| --- | --- | --- |
| 1 | Align | Team has read prior work; personas + screening survey drafted; metrics baselined |
| 2–5 | Understand | 5–8 existing-user interviews; 5 novice first-touch studies; settings card sort. Synthesis: personas + journey maps + prioritised problems |
| 6–8 | Design + iterate | Two parallel workstreams (onboarding; settings IA). 2 usability rounds each (5 users/round) |
| 9 | Hand off | Revised RFCs 0004 + 0006 → `active`; personas added to design guide; engineering picks up via RFC |

## Prototyping

- **Figma** — static flows (settings layout, onboarding screen sequence).
- **Web/WASM** (`dasher-web`) — interactive, where the *feel* of zooming is the
  thing under test. Send novices a link.
- **Native branch** (Windows/Apple/GTK) — only when an input method (switch,
  eye-gaze) requires the real device stack.

## Deliverables → where they land

- **Personas, journey maps, findings** → this `research/` folder.
- **Validated settings IA** → RFC 0006 detailed design.
- **Validated onboarding mechanism** → RFC 0004 detailed design (may be unlike
  anything currently on the list — that's the point).
- **Cross-platform parity** preserved by routing every design through an RFC
  that maintainers review.

## Operating rules

- One finding doc per study, committed here.
- No design lands in a frontend without an accepted RFC (prevents one-platform
  drift).
- If research overturns a current assumption (e.g. "don't use Game Mode"), say
  so explicitly in the RFC revision — that's a success, not a failure.

## How to update this file

This is a living plan. Edit it as scope/roles/timeline shift; date-stamp the
top. Major scope changes go through a governance note, not silently.
