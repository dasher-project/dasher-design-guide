# Welcome, UX volunteer 👋

Welcome to Dasher, and thank you for giving your time. This is the document we
wish every new contributor could read first. It explains **what Dasher is, why
this matters, and how you can help** — in plain language, no engineering
background required.

> You're contributing in a personal capacity, independent of any employer.
> This is a community project and we're glad you're here.

---

## What is Dasher?

**Dasher is a different way to type.** Instead of pressing keys, you *steer*
toward the letter you want: letters sit in boxes that zoom toward a point on
screen, and you guide that point to "write" by moving your pointer (a mouse,
your finger, your eyes, or a switch). The more likely a letter is, the bigger
its box — so common words flow quickly.

It was invented at Cambridge around 25 years ago by the physicist and science
communicator **David MacKay** and colleagues. The clever part is that the
zooming is driven by *probability* — letters that are likely to come next are
given more room, so the language itself helps you write. It was built
originally for people who can't easily use a keyboard — people living with
MND/ALS, cerebral palsy, spinal injury, or who communicate via eye-gaze or
switches. It's **free and open source**, and runs on Apple, Windows, Linux/GTK,
Android, and the web.

The magic of Dasher is that once it "clicks", it feels like the letters are
coming to you. Our job is to get more people to that "click" — because today,
most don't.

## See Dasher in action

Dasher is much easier to grasp in two minutes of video than in any amount of
text, so please take a look before we talk:

- **[David MacKay's talk](https://dasher.at/docs/research/presentations/)** — start here. It's the best
  explanation of how Dasher works and why, given by one of its inventors (the
  talk at the top of that page).
- **[User demonstration videos](https://dasher.at/about/#demonstrations)** — real people writing with Dasher
  using a mouse, their eyes, and switches. This is who we're designing for.
- **[Dasher's history and purpose](https://dasher.at/about/)** — background for when you'd like to go a
  little deeper.

## Why we need you

The project is in **great shape technically**: a clean, well-tested engine at
the core, a tidy C API that every frontend shares, and good governance. What's
left is the human side — the **user experience** — and that's the hard part.

Dasher is powerful, but it has a steep learning curve. New users frequently
describe the first minute as "sea-sickness inducing", and a lot of people give
up before they ever get productive. The people who *do* get it tend to be
either quite tech-literate and persistent, or lucky enough to have an expert
sit with them. **We want to shorten that gap** so far more people can pick
Dasher up and benefit from it.

That's a UX problem, not an engineering one — which is why your help is
genuinely valuable. There are real users, a real product, and a real chance to
make communication easier for people who need it. It's meaningful work, and
it's fun: Dasher is a strange, elegant idea, and you'll be helping shape how
people first meet it.

## What this effort is about

A focused, time-boxed sprint (8–10 weeks) on three things, all of which users
have told us hurt:

1. **The very first experience** — what happens the moment someone opens Dasher
   for the first time. Right now: nothing. No welcome, no "here's how it
   works", no practice. You're dropped straight into the live tool.
2. **The settings** — Dasher has over a hundred settings. For experts that's
   power; for newcomers it's overwhelming. We need to work out what people
   actually need to see and when.
3. **Training and gamification** — even once the idea clicks, building speed
   takes practice. We want to explore game-like training modes that make
   practice engaging and accessible for eye-gaze, switch, and touch users.

## The one rule: we don't know the answers yet

We have **hunches** — for example, "maybe a short practice mode would help
people get the feel", or "maybe a quick 'watch how this works' moment would
orient them". But nothing is decided, and history tells us our hunches are
often wrong.

So this is **research, not validation**. Your job is to help us discover what
actually works for real users. We might end up building something none of us
have on the list today. If your research overturns our assumptions, that's a
win — please say so loudly.

(Note for the curious: there *used* to be an automated "demo mode" in the
engine. It was removed because it crashed. We might build something like it
again, done properly — or we might find a better idea. That decision follows
the research, not the other way around. Don't worry about the internals.)

## Who we need to talk to

**Both brand-new users and experienced ones** — because they answer different
questions, and we need both.

- **Brand-new users** tell us about the *first-touch* struggle — where people
  stall, what confuses them, what makes them give up. Existing users can't
  answer this well: they got over the hump long ago and have forgotten what was
  hard. We'll recruit newcomers via social media, and also try to reach people
  who are newer to technology through AAC communities, clinics, and device
  makers (so we don't only hear from the tech-savvy).
- **Experienced users** tell us what seasoned users value, where the settings
  hurt in daily use, and what "good" looks like once you're fluent.

We also want to cover the different **ways people use Dasher** — mouse, touch,
eye-gaze, and switch — because each is a different experience with different
needs.

## What does "success" look like?

Honestly: **we're not sure yet, and figuring that out is part of the work.**
The top-line goal is clear — *more people get productive with Dasher, faster,
and stick with it* — but the specific things we measure need to be defined, and
that definition should come from listening to both new and existing users.

Some candidate measures we might settle on (not decisions, just starters):

- How long until a new user writes their first sentence?
- How many complete a first practice session vs. give up halfway?
- Do people come back the next day? The next week? *(This is probably the
  truest sign we've closed the gap.)*
- Can people find a setting they're looking for without help?

We'll agree the final list together early in the sprint.

## How we'll work together

We organise into **three squads**, each owning one problem area:

- **Squad A — Onboarding & First-Time Experience.** Design a seamless tutorial
  and setup process that makes the first five minutes of using Dasher
  effortless.
- **Squad B — Settings & Configuration Architecture.** Simplify and group
  Dasher's extensive engine settings so users can easily customise their
  experience without getting lost.
- **Squad C — Gamification & Training Mode.** Design structured, engaging
  training exercises/games to help users build typing speed and accuracy —
  working closely with Squad A so training bridges naturally from onboarding.

**Each squad has an embedded end user** — an active Dasher user who's there
throughout the sprint, not just at test time. They take part in your research,
test your wireframes, and give you immediate, real-world feedback. Their voice
carries weight when it comes to settling on recommendations.

Roles within a squad are **things to do, not titles for one person** — several
of you will want to run interviews, and several will want to prototype, and
that's great. We sort out who does what in the kickoff.

- **Research lead (volunteer)** — shapes the research approach, consent, and how
  we turn findings into evidence.
- **Recruit & ops (project lead)** — I handle recruitment calls, screening,
  scheduling, consent, and storing recordings safely and privately.
- **Interviewers / facilitators** — talk to users, run the studies.
- **Synthesis** — turn recordings and notes into clear findings.
- **Prototyping** — sketch ideas in Figma; build clickable things; for the
  parts where the *feel* of Dasher matters, we can put a real Dasher in a web
  browser so anyone can try a prototype with a link.

### The cadence

We respect your time as volunteers. We operate on a **bi-weekly Tuesday**
cycle:

- **Every other Tuesday:** All-hands sync, 1 hour. General updates, squad
  show-and-tells (10 minutes each), cross-squad coordination.
- **Off-Tuesdays:** Your squad runs its own brief check-in with your embedded
  end user. You manage your own tasks — the maintainer doesn't attend unless
  asked.

### Where things live

- **[Shared Google Drive](https://drive.google.com/)** — research tracker
  spreadsheet, user research interview log, working docs. (You'll get access
  in the kickoff.)
- **`research/` folder (this repo)** — the plan, write-ups, and final RFCs.
- **`ux-background/`** — earlier UX thinking to build on.

### How decisions become RFCs

Each squad's research and prototyping leads to an **RFC** — a short written
proposal that the project agrees on before anyone builds it. You either settle
on a draft RFC that already exists (updating it with what you learned) or
propose a new direction. The embedded end user is part of that settlement.
Once the squad agrees, the RFC comes to the whole group for final sign-off.
(See the [plan](plan.md) for the full process.)

We keep this to a focused 8–10 weeks so the commitment is finite. Rough shape
of the weeks: **align** (1-on-1s and squad assembly) → **listen** (interviews,
first-touch studies, settings card-sorting) → **design and test** (sketch,
prototype, settle on RFCs) → **hand off** (group agreement and handover to
engineering).

## Where to start

This is a **continuation**, not a restart — there's already UX thinking to
build on. Good first reads:

- **[plan.md](plan.md)** — the draft plan for how we'll go about this work
  (phases, methods, who we'll talk to). Written in plain language, and very
  much open to your input.
- `ux-background/Dasher – settings + onboarding.pdf` — earlier thinking on
  these exact two problems.
- `ux-background/Dasher UX milestone 3.pdf` — research from a previous
  milestone.
- The main design guide (`README.md`) — the project's visual and interaction
  reference.

If you want to go deeper into the engineering side later, the changes this work
will inform are tracked as RFC proposals (`governance/rfcs/0004-onboarding.md`
and `0006-settings-ia.md`). Squad C (gamification) may open a new RFC or fold
into the onboarding one — that's a decision for the squad. Don't worry if "RFC"
means nothing to you right now — it's just how the project agrees on changes
across all its platforms, and we'll walk you through it when it matters.

## A last word

You're joining at the moment Dasher most needs UX help. The foundations are
solid; what's missing is the bridge between a brilliant idea and the people who
could benefit from it. That bridge is what we're building together.

Welcome aboard. 🎉
