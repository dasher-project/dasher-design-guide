---
version: "alpha"
name: Dasher v6.0
description: >-
  Visual identity for Dasher, a predictive continuous-gesture text-entry system
  built for accessibility. Extracted from the fixed Dasher logo with WCAG AA/AAA
  contrast adjustments.
colors:
  primary: "#99D4CD"
  secondary: "#F8E063"
  tertiary: "#EB5B5C"
  text: "#0F4B75"
  bg-light: "#F4F7F6"
  surface-light: "#FFFFFF"
  border-light: "#E0E6E8"
  highlight-light: "#E9F2F1"
  bg-dark: "#12181B"
  surface-dark: "#1E262B"
  border-dark: "#2A353D"
  highlight-dark: "#1D2D35"
typography:
  h1:
    fontFamily: Inter
    fontSize: 1.5rem
    fontWeight: "600"
    lineHeight: 1.3
  h2:
    fontFamily: Inter
    fontSize: 1rem
    fontWeight: "500"
    lineHeight: 1.35
  body:
    fontFamily: Inter
    fontSize: 0.875rem
    fontWeight: "400"
    lineHeight: 1.5
  caption:
    fontFamily: Inter
    fontSize: 0.75rem
    fontWeight: "300"
    lineHeight: 1.4
  glyph:
    fontFamily: Arial
    fontSize: 1rem
    fontWeight: "700"
    fontFeature: "tnum"
rounded:
  sm: 4px
  md: 8px
  lg: 12px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.text}"
    rounded: "{rounded.md}"
    padding: 12px
  button-alert:
    backgroundColor: "{colors.tertiary}"
    textColor: "#FFFFFF"
    rounded: "{rounded.md}"
    padding: 12px
  button-highlight:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.text}"
    rounded: "{rounded.md}"
    padding: 12px
  surface-light:
    backgroundColor: "{colors.surface-light}"
    textColor: "{colors.text}"
  surface-dark:
    backgroundColor: "{colors.surface-dark}"
    textColor: "#FFFFFF"
  toolbar-top:
    height: 64px
  status-bar-bottom:
    height: 48px
  touch-target:
    size: 48px
---

## Overview

Dasher v6.0 is an accessibility-first design system for a predictive,
continuous-gesture text-entry application. The palette is directly extracted from
the fixed Dasher logo — four distinctive colors that represent the software's
zooming-mechanic character nodes. The system prioritizes legibility under
continuous-zooming conditions, generous touch targets for assistive devices, and
reduced visual load to prevent disorientation.

An agent that reads this file will produce a UI with Deep Navy text on warm
light-grey backgrounds, Dasher Teal primary actions, Warm Yellow zooming
highlights, and Coral Red alerts — all meeting WCAG AA contrast ratios.

### Cross-Platform Notes

Dasher runs on multiple platforms (Web/Electron, macOS/iOS via SwiftUI,
Windows/Linux via Avalonia, Linux/GNOME via GTK), all backed by DasherCore.
The tokens in this file are **platform-agnostic**. Each frontend maps these
values to native equivalents. Platform-specific visual deviations (native
controls, OS conventions) are allowed, but color values, spacing, touch-target
sizes, and interaction patterns must match the tokens defined here.

### Updating This File

This file is the **normative source of truth** for design tokens. When a design
decision changes:

1. Update the YAML front matter tokens first.
2. Update the corresponding prose sections to match.
3. Run `npx @google/design.md lint DESIGN.md` — resolve all errors before
   committing.
4. Update README.md to reflect rationale for the change.

## Colors

The palette is rooted in the four brand colors from the fixed logo, plus a
set of neutral surfaces supporting both light and dark themes.

### Brand Colors

- **Primary / Dasher Teal (`#99D4CD`):** Canvas framing, branding accents,
  primary buttons. The signature mint tone signals interactive elements.
- **Secondary / Warm Yellow (`#F8E063`):** Zooming boxes, current letter
  groupings, interactive hover states. Draws the eye to active canvas regions.
- **Tertiary / Coral Red (`#EB5B5C`):** Target highlight boxes, path
  corrections, error strikes, delete states. High-visibility alert color.
- **Text / Deep Navy (`#0F4B75`):** High-contrast text glyphs, labels, top bar
  iconography. Provides excellent readability on light and dark surfaces.

### Neutrals (Light Theme)

- **Background (`#F4F7F6`):** App layout background — cool, slightly muted.
- **Surface (`#FFFFFF`):** Sidebars, textboxes, settings panels — clean white.
- **Border (`#E0E6E8`):** Structural separations, input borders — subtle.
- **Highlight (`#E9F2F1`):** Secondary action highlights — faint teal tint.

### Neutrals (Dark Theme)

- **Background (`#12181B`):** App layout background — near-black with warmth.
- **Surface (`#1E262B`):** Panels and cards — slightly raised from background.
- **Border (`#2A353D`):** Separations — visible but not distracting.
- **Highlight (`#1D2D35`):** Secondary highlights — muted depth.

## Typography

Two font families serve distinct roles.

### Interface Text (Inter / Google Sans)

Used for menus, status bars, taskbars, preferences, and onboarding prompts.
Inter's wide apertures and distinct letterforms (clear I/l/1 distinction)
reduce eye fatigue during extended use.

| Token       | Size    | Weight     | Use                                    |
| :---------- | :------ | :--------- | :------------------------------------- |
| `h1`        | 1.5rem  | Semi-Bold  | Settings / onboarding headings         |
| `h2`        | 1rem    | Medium     | Subheadings, actionable items          |
| `body`      | 0.875rem| Regular    | Body text, help prompts                |
| `caption`   | 0.75rem | Light/Reg  | Captions, sub-labels                   |

### Canvas Glyphs (Arial / Noto Sans)

Used for letters inside zooming boxes on the interactive canvas. Size is
dynamic (relative to node bounds). Heavy weights preferred for high-speed
tracking. Font smoothing and subpixel rendering must be enabled to prevent
text jitter during high-speed zooming.

## Layout & Spacing

The main application uses a 3-pane responsive layout:

1. **Top Toolbar** — Fixed 64px height. Quick commands and status.
2. **Main Interactive Area** — Fluid height.
   - Left Pane (optional): Zooming Canvas.
   - Right Pane: Standalone Text Editor Window.
3. **Bottom Status Bar** — Fixed 48px height. Real-time adjustment controls.

### Spacing Scale

| Token | Value | Use                              |
| :---- | :---- | :------------------------------- |
| `xs`  | 4px   | Tight internal padding           |
| `sm`  | 8px   | Standard internal padding        |
| `md`  | 16px  | Component spacing                |
| `lg`  | 24px  | Section padding                  |
| `xl`  | 32px  | Page-level margins               |

### Touch Targets

All interactive elements must meet minimum 48 x 48dp dimensions. Hover
activation delay (dwell clicking) must be configurable between 200ms and 800ms.

## Elevation & Depth

Dasher uses minimal elevation to maintain a flat, accessible feel. Surfaces
differentiate through background color shifts rather than heavy shadows.

- **Level 0 (Background):** No shadow. The base layout canvas.
- **Level 1 (Surface):** `0 1px 3px rgba(0,0,0,0.06)` — Sidebars, panels.
- **Level 2 (Raised):** `0 4px 12px rgba(15,75,117,0.15)` — Hover states, modals.

## Shapes

Border radius is used sparingly to maintain a clean, modern aesthetic:

| Token | Value | Use                              |
| :---- | :---- | :------------------------------- |
| `sm`  | 4px   | Chips, tags, small inputs        |
| `md`  | 8px   | Buttons, cards, panels           |
| `lg`  | 12px  | Modals, large containers         |

## Components

### Toolbar (Top)

Fixed 64px bar consolidating macro-actions: New, Open, Save, Play/Pause,
Position, Prefs. Each uses explicit iconography with descriptive tooltips.
Minimum 48px touch targets per icon.

### Status Bar (Bottom)

Fixed 48px bar for micro-adjustments without interrupting text composition:
alphabet selector, speed control, learning mode toggle, color palette switcher,
font size control, speech output control.

### Sidebar Editor Panel

Clipboard and speech actions alongside the text editor: Copy, Copy All, Paste,
Quick Speak. Prominent CTA for vocalization.

### Button (Primary)

Dasher Teal background with Deep Navy text. 48px minimum height. 8px border
radius. Hover/focus adds a Deep Navy border and subtle shadow. Transition uses
Material Design standard easing.

### Settings Modal

Tabbed by usage context: Customization, Punctuation, Volume, Locks,
Accessibility. Includes a **live mini-canvas preview** so users see changes
without closing the dialog.

## Do's and Don'ts

### Do

- **Do** maintain minimum 48px touch targets for all interactive elements.
- **Do** use the four brand colors as the sole accent palette — no extra hues.
- **Do** enable configurable dwell-click delays (200ms–800ms) for assistive devices.
- **Do** provide live preview in settings to reduce open/test/close cycles.
- **Do** use heavy font weights on canvas glyphs for high-speed tracking legibility.
- **Do** suppress sibling node children in beginner mode to reduce visual load.
- **Do** maintain 25% clear-space around the logo at all times.
- **Do** use color harmonization (muted monochromes) for sibling groups on the canvas.

### Don't

- **Don't** alter, stretch, or recolor the fixed Dasher logo.
- **Don't** render the logo below 32px wide — glyph visibility degrades.
- **Don't** place the logo on complex background patterns.
- **Don't** show correction paths all at once — animate them sequentially.
- **Don't** bury language-swap triggers in nested menus — keep them in the status bar.
- **Don't** use pure white (`#FFFFFF`) as a background — use `#F4F7F6` for warmth.
- **Don't** organize settings by content type — group by usage context.
- **Don't** allow canvas text jitter — enable font smoothing and subpixel rendering.
