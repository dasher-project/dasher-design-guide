# UX sprint plan — **draft**

> 🟠 **This is a draft. Everything in it is up for review.** We've written it
> to give us all a shared starting point, not a set of instructions. If you
> think a phase is wrong, a method is missing, or the order should change —
> say so. The plan is ours to shape together in the kickoff, and to keep
> adjusting as we learn.
>
> Companion to the **[welcome README](README.md)** — read that first if you
> haven't; this is the "how we'll actually go about it" detail.

## The three problems we're tackling

1. **The first-run experience.** Right now someone opening Dasher for the first
   time gets no welcome, no explanation, and no practice — they're dropped
   straight into the live tool. We want to fix that.
2. **The settings.** Dasher has over a hundred settings. Powerful for experts,
   overwhelming for newcomers. We want people to see what they need, when they
   need it — no more, no less.
3. **Training and gamification.** Even once someone understands the idea,
   building speed and accuracy takes practice. We want to explore game-like
   training modes that make practice engaging — and critically, accessible for
   the input methods our users actually rely on (eye-gaze, switch, touch).

## How we'll approach it

**Listen before we design, and test before we decide.** We have hunches, but
we expect them to be wrong in interesting ways. The plan below is built around
*finding out* rather than *delivering a pre-decided answer*.

We organise into **three squads**, each owning one of the problems above. Each
squad has an **embedded end user** — an active Dasher user who's there
throughout, not just at test time. They ground every decision in real-world
need.

There are **four phases** over roughly 8–10 weeks. Timings are approximate and
will flex.

### Phase 1 — Get aligned (about 1–2 weeks)

We get on the same page and find our footing as a team. Three things happen:

- **Everyone reads the existing thinking.** (See "where to start" in the
  welcome.) The `ux-background/` PDFs and this plan are the shared starting
  point — come with questions and challenges.
- **1-on-1 discovery calls.** The maintainer schedules a short (30-minute) chat
  with each volunteer. We share the project brief, learn what you're interested
  in (research, UI design, prototyping, gamification), and confirm your
  bi-weekly Tuesday availability. We also ask: *"Are you comfortable working in
  a peer-pair with another designer and an end user?"*
- **Squad assembly and kickoff.** We group volunteers into three squads based
  on interests, assign one embedded end user to each, and hold the first
  all-hands Tuesday meeting to walk through templates, workflow, and the shared
  Google Drive.

By the end of Phase 1, every squad knows its focus, its end user, and its
first research targets.

### Phase 2 — Listen (about 3–4 weeks)

This is the heart of it. Each squad talks to people and watches them use
Dasher, focused on their problem area. The squads run in parallel:

- **Squad A (Onboarding)** interviews end users about their first memory and
  struggles learning Dasher. What was the moment it clicked — or the moment
  they nearly gave up?
- **Squad B (Settings)** documents the current settings across platforms
  (Linux, iOS/macOS, Android), then runs **card-sorting exercises** with users:
  lay the settings on cards, let people group them however makes sense. The
  structure comes from users, not from our guesses.
- **Squad C (Gamification)** researches typing-game mechanics that adapt to
  accessibility inputs, and interviews users about what would make practice
  feel rewarding rather than frustrating. They coordinate closely with Squad A
  so training bridges naturally from onboarding.

We do this in **small groups, often** — roughly five people per round — rather
than one big batch. Small groups are easier to arrange and quicker to learn
from, and running rounds often means we catch mistakes early.

At the end of this phase, each squad pulls its findings together into: short
descriptions of the different kinds of people who use Dasher ("personas"), a
picture of the journey a new user goes on, and a plain-language list of the
biggest problems in their area — ranked.

### Phase 3 — Design and test (about 3 weeks)

Each squad picks its top problems and starts sketching answers — first rough,
then more real. For each idea the squad:

1. Sketches it (on paper or in a design tool).
2. Turns it into something people can try — a clickable mock, or for the parts
   where the *feel* of Dasher matters, a real Dasher running in a web browser
   that people can reach via a link.
3. Watches a few people use it (starting with the embedded end user), notes
   what confuses them, and improves it.
4. Repeats. Usually two rounds of testing per idea is enough to get
   confidence.

**The output of this phase is an RFC (or a revision of an existing one).**
Each squad takes what they've learned and either settles on one of the draft
RFCs that already exist, or writes a new one. The embedded end user is part of
that — they've been there through the testing, and their voice carries weight
in the recommendation. The squad agrees on the RFC internally before bringing
it to the wider group.

### Phase 4 — Hand off (about 1 week)

We come together as a whole group. Each squad presents its RFC — what they
found, what they recommend, and why. We agree the way forward collectively,
with end users in the room. Those agreed RFCs then go into the project's normal
engineering pipeline. No code changes happen in this sprint — our output is
evidence, design, and agreed proposals.

## The cadence

We respect your time as volunteers. We operate on a **bi-weekly Tuesday**
cycle:

**Alternate Tuesdays (all-hands, 1 hour, maintainer-led):**

| Time | What |
|:---|:---|
| 0:00 – 0:15 | General project updates, RFC alignment, technical constraints. |
| 0:15 – 0:45 | Squad updates — 10 minutes per squad showing work (Google Docs, Figma, prototypes). |
| 0:45 – 1:00 | Next steps, blocker clearing, cross-squad coordination. |

**Off-Tuesdays (squad-level, self-managed):**

Each squad schedules its own brief sync to review work, assign peer tasks, and
discuss concepts directly with their embedded end user. The maintainer doesn't
attend unless asked — the squads run themselves.

```
          [ You (Maintainer) ]
                   │
       ┌───────────┼───────────┐  (Every other Tuesday: 1-hour all-hands)
       ▼           ▼           ▼
  [Squad A]   [Squad B]   [Squad C]
 (Onboarding) (Settings) (Gamification)
       │           │           │
 [End User]  [End User]  [End User]   (Embedded in each squad)
```

## Who we'll talk to

**Both brand-new and experienced users** — they answer different questions, and
we need both. (The welcome explains why.)

- **Brand-new users** — reached through social media, and we'll also try hard
  to reach people who are newer to technology, through AAC communities,
  clinics, and device makers, so we don't only hear from the tech-savvy.
- **Experienced users** — from our existing group of keen users.

Across everyone we talk to, we want to cover the different **ways people use
Dasher**: mouse, touch, eye-gaze, and switch. These are genuinely different
experiences with different needs — especially for eye-gaze and switch users,
where we'll need to test on the real thing rather than in a browser.

## What we'll produce

- **Write-ups of what we learned** from each round of conversations and tests.
- **Descriptions of our users** (the "personas") and the journeys they go on.
- **Sketches and prototypes** of the ideas we settle on.
- **Agreed RFCs** — one per squad — with the evidence behind them, ready for
  engineering to pick up.

All of this lives in this `research/` folder (and the shared Google Drive), so
it's there for everyone to see and build on later.

## How decisions become changes

This project runs on more than one platform (Apple, Windows, Linux, Android,
web), so a change has to work for all of them. The project's way of handling
that is a short written proposal — called an **RFC** — that the maintainers
look at and agree before anyone builds it. (If "RFC" is new to you, don't
worry — it's just "write the idea down clearly, get agreement, then build.")

Our recommendations feed into proposals that already exist and are waiting for
exactly this kind of input:

- **`governance/rfcs/0004-onboarding.md`** — the first-run experience (Squad A).
- **`governance/rfcs/0006-settings-ia.md`** — the settings (Squad B).
- Squad C may open a new RFC for training/gamification, or fold into the
  onboarding one — that's a decision for the squad.

Each squad either settles on the existing RFC (updating it with what they
learned) or proposes a new direction. The embedded end user is part of that
settlement. Once the squad agrees internally, the RFC comes to the whole group
in Phase 4 for final sign-off.

## How we'll work together

Roles are things to do, not one person each — several of you may want to run
interviews or build prototypes within a squad. We sort out who does what in the
kickoff. (The welcome has the role list.) Squads are self-organising between
all-hands Tuesdays, and the maintainer is there to unblock, not to direct.

## This is a draft — please mark it up

The phases, the methods, the numbers of people, the order of things — all of
it is a starting point. Bring your changes to the kickoff (or jot them in this
document). A good plan is one the whole group has shaped and believes in.
