# UX sprint plan — **draft**

> 🟠 **This is a draft. Everything in it is up for review.** We've written it
> to give us all a shared starting point, not a set of instructions. If you
> think a phase is wrong, a method is missing, or the order should change —
> say so. The plan is ours to shape together in the kickoff, and to keep
> adjusting as we learn.
>
> Companion to the **[welcome README](README.md)** — read that first if you
> haven't; this is the "how we'll actually go about it" detail.

## The two problems we're tackling

1. **The first-run experience.** Right now someone opening Dasher for the first
   time gets no welcome, no explanation, and no practice — they're dropped
   straight into the live tool. We want to fix that.
2. **The settings.** Dasher has over a hundred settings. Powerful for experts,
   overwhelming for newcomers. We want people to see what they need, when they
   need it — no more, no less.

## How we'll approach it

**Listen before we design, and test before we decide.** We have hunches, but
we expect them to be wrong in interesting ways. The plan below is built around
*finding out* rather than *delivering a pre-decided answer*.

There are **four phases** over roughly 8–10 weeks. Timings are approximate and
will flex.

### Phase 1 — Get aligned (about 1 week)

We get on the same page: everyone reads the existing thinking (see "where to
start" in the welcome), we agree who's doing what, and we agree how we'll know
whether we've succeeded (see "what does success look like" — itself something
we settle here, with input from both new and existing users).

### Phase 2 — Listen (about 3–4 weeks)

This is the heart of it. We talk to people and watch them use Dasher. Three
things happen in parallel:

- **Conversations with experienced users.** We sit with (or screen-share with)
  people who use Dasher regularly, watch them work, and ask where it frustrates
  them — especially in the settings.
- **First-touch studies with brand-new users.** We find people who've never
  used Dasher, hand it to them cold, and watch where they stall. (They can just
  open a link in a browser — nothing to install.) We ask them to think out loud
  as they go.
- **A settings sorting exercise.** We put the settings onto "cards" and ask
  people to group them in whatever way makes sense to them — so the
  *structure* of the settings comes from users, not from our guesses.
  Afterwards we check: if we lay things out the way people suggested, can
  someone actually find a given setting?

We do this in **small groups, often** — roughly five people per round — rather
than one big batch. Small groups are easier to arrange and quicker to learn
from, and running rounds often means we catch mistakes early.

At the end of this phase we pull it all together into: short descriptions of
the different kinds of people who use Dasher (often called "personas"), a
picture of the journey a new user goes on, and a plain-language list of the
biggest problems — ranked.

### Phase 3 — Design and test (about 3 weeks)

We pick the top problems and start sketching answers — first rough, then more
real. For each idea we:

1. Sketch it (on paper or in a design tool).
2. Turn it into something people can try — a clickable mock, or for the parts
   where the *feel* of Dasher matters, a real Dasher running in a web browser
   that people can reach via a link.
3. Watch a few people use it, note what confuses them, and improve it.
4. Repeat. Usually two rounds of testing per idea is enough to get
   confidence.

The two workstreams (first-run experience, and settings) can run at the same
time, with different people leading each.

### Phase 4 — Hand off (about 1 week)

We write up what we learned, what we recommend, and why. Those
recommendations then go into the project's normal way of agreeing changes
(described below). No code changes happen in this sprint — our output is
evidence and design, and the engineering side picks it up from there.

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
- **Clear recommendations**, with the evidence behind them.

All of this lives in this `research/` folder, so it's there for everyone to see
and build on later.

## How decisions become changes

This project runs on more than one platform (Apple, Windows, Linux, Android,
web), so a change has to work for all of them. The project's way of handling
that is a short written proposal — called an "RFC" — that the maintainers look
at and agree before anyone builds it. (If "RFC" is new to you, don't worry —
it's just "write the idea down clearly, get agreement, then build.")

Our recommendations feed into two proposals that already exist and are waiting
for exactly this kind of input — one about the first-run experience, one about
the settings. We'll handle the mechanics of that; your focus is the research
and the design.

## How we'll work together

Roles are things to do, not one person each — several of you may want to run
interviews or build prototypes. We sort out who does what in the kickoff. (The
welcome has the role list.) We meet once a week for about 45 minutes and chat
async in between, for a focused 8–10 weeks.

## This is a draft — please mark it up

The phases, the methods, the numbers of people, the order of things — all of
it is a starting point. Bring your changes to the kickoff (or jot them in this
document). A good plan is one the whole group has shaped and believes in.
