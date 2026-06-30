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

A focused, time-boxed sprint (8–10 weeks) on two things, both of which users
have told us hurt:

1. **The very first experience** — what happens the moment someone opens Dasher
   for the first time. Right now: nothing. No welcome, no "here's how it
   works", no practice. You're dropped straight into the live tool.
2. **The settings** — Dasher has over a hundred settings. For experts that's
   power; for newcomers it's overwhelming. We need to work out what people
   actually need to see and when.

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

Roles here are **things to do, not titles for one person** — several of you
will want to run interviews, and several will want to prototype, and that's
great. We sort out who does what in the kickoff.

- **Research lead (volunteer)** — shapes the research approach, consent, and how
  we turn findings into evidence.
- **Recruit & ops (project lead)** — I handle recruitment calls, screening,
  scheduling, consent, and storing recordings safely and privately.
- **Interviewers / facilitators** — talk to users, run the studies.
- **Synthesis** — turn recordings and notes into clear findings.
- **Prototyping** — sketch ideas in Figma; build clickable things; for the
  parts where the *feel* of Dasher matters, we can put a real Dasher in a web
  browser so anyone can try a prototype with a link.

We meet once a week for ~45 minutes, chat async in between, and keep this to a
focused 8–10 weeks so the commitment is finite.

Rough shape of the weeks: **align** (we get on the same page) → **listen**
(interviews and first-touch studies with both cohorts; a settings exercise
where users show us how they'd group the options) → **design and test**
(sketch, prototype, test with real people, repeat) → **hand off** (write up
what we learned and what to build).

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
and `0006-settings-ia.md`). Don't worry if "RFC" means nothing to you right now
— it's just how the project agrees on changes across all its platforms, and
we'll walk you through it when it matters.

## A last word

You're joining at the moment Dasher most needs UX help. The foundations are
solid; what's missing is the bridge between a brilliant idea and the people who
could benefit from it. That bridge is what we're building together.

Welcome aboard. 🎉
