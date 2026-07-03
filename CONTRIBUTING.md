# Contributing to Dasher

Thanks for your interest in contributing. This guide covers both **design/UX**
and **engineering** contributions.

## Where things live

| Path | What |
|:---|:---|
| `DESIGN.md` | Machine-readable design tokens (colors, typography, spacing). **Single source of truth** for all platforms. |
| `README.md` | Human-readable design guide. Sections marked `<!-- GENERATE:... -->` are auto-generated from DESIGN.md — do not edit by hand. |
| `research/` | UX research: volunteer welcome, sprint plan, findings, and RFC drafts. Start at [`research/README.md`](research/README.md). |
| `ux-background/` | Earlier UX thinking (PDFs, decks) to build on. |
| `assets/` | Logo, icon, and design reference images. |

## UX volunteers

If you're here to help with UX research or design:

1. Read **[research/README.md](research/README.md)** — the volunteer welcome.
2. Read **[research/plan.md](research/plan.md)** — the sprint plan and squad structure.
3. You'll get access to the shared Google Drive (research tracker, interview log) during onboarding.

You don't need to understand the engineering side to contribute. Your work
happens in `research/` and the Google Drive.

## Design token changes

If you're changing colours, typography, spacing, or component values:

1. Edit **`DESIGN.md`** YAML front matter (the normative source).
2. Update the prose sections below the YAML to match.
3. Lint: `npm run lint` (must pass with zero errors).
4. Regenerate README.md: `npm run generate`.
5. Commit both `DESIGN.md` and `README.md` together.

Do not edit `<!-- GENERATE:... -->` sections of README.md directly — they are
overwritten.

## The RFC process

Dasher runs on multiple platforms (Apple, Windows, Linux, Android, web). Any
change that affects more than one platform goes through a written **RFC**
(Request for Comments) proposal before it's built.

- Draft RFCs live in `governance/rfcs/` in the main Dasher repository.
- UX squads settle on an RFC (or a revision of one) as the output of their
  research, with their embedded end user as part of that settlement.
- Once a squad agrees internally, the RFC goes to the whole group for sign-off.
- Only after agreement does engineering pick it up.

If you're proposing a design change that has platform implications, open or
update an RFC. If "RFC" is new to you, the maintainer will help — it's just
"write the idea down clearly, get agreement, then build."

## Engineering contributions

For code changes to this repository (scripts, config, docs tooling):

1. Open an issue describing the change.
2. Branch from `main`, make your change.
3. If you touched `DESIGN.md`, run `npm run lint && npm run generate`.
4. Open a pull request with a clear description.

## Questions?

- **UX / research:** start in [`research/`](research/).
- **Design tokens:** check [`DESIGN.md`](DESIGN.md).
- **Anything else:** open an issue.
