---
version: alpha
name: Blok
description: A neo-brutalist design system. Thick outlines, hard offset shadows, flat loud fills and square corners.
colors:
  primary: "#FFE600"
  primary-hover: "#FFD500"
  primary-foreground: "#000000"
  background: "#FFFDF7"
  foreground: "#000000"
  card: "#FFFFFF"
  card-foreground: "#000000"
  popover: "#FFFFFF"
  popover-foreground: "#000000"
  secondary: "#F1EEE5"
  secondary-foreground: "#000000"
  muted: "#F1EEE5"
  muted-foreground: "#525252"
  accent: "#F1EEE5"
  accent-foreground: "#000000"
  destructive: "#D7261D"
  destructive-foreground: "#FFFFFF"
  success: "#00C853"
  success-foreground: "#000000"
  warning: "#FF8A00"
  warning-foreground: "#000000"
  pink: "#FF5CA8"
  pink-foreground: "#000000"
  blue: "#2D5BFF"
  blue-foreground: "#FFFFFF"
  mint: "#5EEAD4"
  mint-foreground: "#000000"
  chart-1: "#FFE600"
  chart-2: "#FF5CA8"
  chart-3: "#2D5BFF"
  chart-4: "#5EEAD4"
  chart-5: "#000000"
  border: "#000000"
  input: "#000000"
  ring: "#2D5BFF"
  grid: "#0000001A"
typography:
  display:
    fontFamily: Archivo
    fontSize: 80px
    fontWeight: 900
    lineHeight: 80px
    letterSpacing: -0.02em
    fontStretch: 125%
  h1:
    fontFamily: Archivo
    fontSize: 56px
    fontWeight: 800
    lineHeight: 56px
    letterSpacing: -0.02em
    fontStretch: 125%
  h2:
    fontFamily: Archivo
    fontSize: 40px
    fontWeight: 800
    lineHeight: 44px
    letterSpacing: -0.015em
    fontStretch: 125%
  h3:
    fontFamily: Archivo
    fontSize: 28px
    fontWeight: 800
    lineHeight: 32px
    letterSpacing: -0.01em
    fontStretch: 125%
  title:
    fontFamily: Archivo
    fontSize: 20px
    fontWeight: 700
    lineHeight: 24px
  body:
    fontFamily: Archivo
    fontSize: 16px
    fontWeight: 400
    lineHeight: 24px
  button:
    fontFamily: Archivo
    fontSize: 16px
    fontWeight: 700
    lineHeight: 24px
  small:
    fontFamily: Archivo
    fontSize: 14px
    fontWeight: 400
    lineHeight: 20px
  ui:
    fontFamily: Archivo
    fontSize: 14px
    fontWeight: 600
    lineHeight: 20px
  caption:
    fontFamily: Space Mono
    fontSize: 12px
    fontWeight: 400
    lineHeight: 16px
    letterSpacing: 0.02em
  label:
    fontFamily: Space Mono
    fontSize: 12px
    fontWeight: 700
    lineHeight: 16px
    letterSpacing: 0.08em
    textTransform: uppercase
  mono:
    fontFamily: Space Mono
    fontSize: 14px
    fontWeight: 400
    lineHeight: 20px
rounded:
  none: 0px
  full: 9999px
spacing:
  "1": 4px
  "2": 8px
  "3": 12px
  "4": 16px
  "5": 20px
  "6": 24px
  "8": 32px
  "12": 48px
  "16": 64px
  "24": 96px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.primary-foreground}"
    borderColor: "{colors.border}"
    borderWidth: 2px
    typography: "{typography.button}"
    rounded: "{rounded.none}"
    height: 48px
    padding: 0 24px
    shadow: 4px 4px 0 0 {colors.foreground}
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    shadow: 6px 6px 0 0 {colors.foreground}
    transform: translate(-2px, -2px)
  button-primary-active:
    shadow: none
    transform: translate(4px, 4px)
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.secondary-foreground}"
    borderColor: "{colors.border}"
    borderWidth: 2px
    typography: "{typography.button}"
    height: 48px
    padding: 0 24px
    shadow: 4px 4px 0 0 {colors.foreground}
  button-outline:
    backgroundColor: "{colors.card}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.border}"
    borderWidth: 2px
    typography: "{typography.button}"
    height: 48px
    padding: 0 24px
    shadow: 4px 4px 0 0 {colors.foreground}
  icon-button:
    backgroundColor: "{colors.card}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.border}"
    borderWidth: 2px
    size: 48px
    shadow: 4px 4px 0 0 {colors.foreground}
  chip:
    backgroundColor: "{colors.card}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.border}"
    borderWidth: 2px
    typography: "{typography.ui}"
    height: 40px
    padding: 0 16px
    shadow: 4px 4px 0 0 {colors.foreground}
  chip-selected:
    backgroundColor: "{colors.foreground}"
    textColor: "{colors.background}"
    shadow: none
    transform: translate(4px, 4px)
  toggle:
    backgroundColor: "{colors.card}"
    borderColor: "{colors.border}"
    borderWidth: 2px
    width: 56px
    height: 32px
    shadow: 4px 4px 0 0 {colors.foreground}
  toggle-checked:
    backgroundColor: "{colors.primary}"
  text-field:
    backgroundColor: "{colors.card}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.input}"
    borderWidth: 2px
    typography: "{typography.body}"
    height: 48px
    padding: 0 16px
    shadow: 4px 4px 0 0 {colors.foreground}
  badge:
    borderColor: "{colors.border}"
    borderWidth: 2px
    typography: "{typography.label}"
    height: 28px
    padding: 0 10px
  card:
    backgroundColor: "{colors.card}"
    textColor: "{colors.card-foreground}"
    borderColor: "{colors.border}"
    borderWidth: 3px
    rounded: "{rounded.none}"
    padding: 20px
    shadow: 6px 6px 0 0 {colors.foreground}
  card-header:
    borderColor: "{colors.border}"
    borderWidth: 3px
    typography: "{typography.label}"
    padding: 12px 16px
  sticker:
    borderColor: "{colors.border}"
    borderWidth: 2px
    typography: "{typography.label}"
    padding: 6px 12px
    rotate: -6deg
    shadow: 4px 4px 0 0 {colors.foreground}
  toast:
    backgroundColor: "{colors.card}"
    borderColor: "{colors.border}"
    borderWidth: 2px
    padding: 12px 8px 12px 16px
    shadow: 10px 10px 0 0 {colors.foreground}
  marquee:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.primary-foreground}"
    borderColor: "{colors.border}"
    borderWidth: 3px
    typography: "{typography.h3}"
    padding: 12px 0
---

# Blok

## Overview

Blok is a neo-brutalist system for marketing sites, launches, events, indie products and creative tools. Everything is a block: a flat fill inside a 2px black outline (3px on cards), a hard shadow offset down and right with no blur, square corners, heavy type. Blocks are physical: on hover a block lifts and its shadow grows, on press it sinks into its shadow. The page behind the blocks shows its grid.

Loud but disciplined. There are five fills (a high-visibility yellow for the primary action, a hot pink, a cobalt blue, a mint and black), two offsets for shadows (4px on controls, 6px on cards), one outline color, one radius (none) and one focus color. The same values appear everywhere.

The same tokens exist in three places and must stay in sync:

- `blok.css` for Tailwind CSS v4. Token names follow shadcn/ui.
- This file, for people and coding agents.
- The Figma library "Blok Design System" (variables, text styles, components).

When building with Blok, use the semantic tokens and the recipes under Components. If a screen needs something this file does not cover, build it from the same parts: a 2px outline, a 4px or 6px hard shadow in `foreground`, a flat fill from the five, Archivo for words and Space Mono in capitals for labels.

## Colors

Use semantic tokens only. The default Tailwind palette is removed in `blok.css`, so `bg-blue-500` and similar classes produce nothing; the loud fills are `bg-pink`, `bg-blue` and `bg-mint`.

| Token | Light | Dark | Use |
| --- | --- | --- | --- |
| `background` | `#FFFDF7` | `#121212` | Page ground, text on inverted blocks |
| `foreground` | `#000000` | `#F5F2E8` | Text, icons, outlines, shadows, inverted blocks |
| `card` | `#FFFFFF` | `#1B1B1B` | Cards, controls, fields, header bar |
| `card-foreground` | `#000000` | `#F5F2E8` | Text on cards |
| `popover` | `#FFFFFF` | `#1B1B1B` | Menus, popovers, dialogs, toasts |
| `popover-foreground` | `#000000` | `#F5F2E8` | Text on popovers |
| `primary` | `#FFE600` | `#FFE600` | The main action, the on state of toggle, slider, checkbox and radio, the marquee |
| `primary-hover` | `#FFD500` | `#FFD500` | Hover fill for primary |
| `primary-foreground` | `#000000` | `#000000` | Text on primary; always black |
| `secondary` | `#F1EEE5` | `#2A2A2A` | Secondary buttons, quiet surfaces |
| `secondary-foreground` | `#000000` | `#F5F2E8` | Text on secondary |
| `muted` | `#F1EEE5` | `#2A2A2A` | Surface behind grouped content, code blocks |
| `muted-foreground` | `#525252` | `#B8B4A8` | Secondary text, captions, times and prices |
| `accent` | `#F1EEE5` | `#2A2A2A` | Hover surface for outline and icon buttons |
| `accent-foreground` | `#000000` | `#F5F2E8` | Text on accent |
| `destructive` | `#D7261D` | `#D7261D` | Errors and destructive actions |
| `destructive-foreground` | `#FFFFFF` | `#FFFFFF` | Text on destructive |
| `success` | `#00C853` | `#00C853` | Success fill and dot |
| `success-foreground` | `#000000` | `#000000` | Text on success |
| `warning` | `#FF8A00` | `#FF8A00` | Warning fill, callout, badge |
| `warning-foreground` | `#000000` | `#000000` | Text on warning |
| `pink` | `#FF5CA8` | `#FF5CA8` | Loud fill: card headers, stickers, badges |
| `pink-foreground` | `#000000` | `#000000` | Text on pink |
| `blue` | `#2D5BFF` | `#2D5BFF` | Loud fill: card headers, badges |
| `blue-foreground` | `#FFFFFF` | `#FFFFFF` | Text on blue; always white |
| `mint` | `#5EEAD4` | `#5EEAD4` | Loud fill: card headers, callouts, badges, toast stripe |
| `mint-foreground` | `#000000` | `#000000` | Text on mint |
| `chart-1` | `#FFE600` | `#FFE600` | First data series |
| `chart-2` | `#FF5CA8` | `#FF5CA8` | Second data series |
| `chart-3` | `#2D5BFF` | `#2D5BFF` | Third data series |
| `chart-4` | `#5EEAD4` | `#5EEAD4` | Fourth data series |
| `chart-5` | `#000000` | `#F5F2E8` | Fifth data series |
| `border` | `#000000` | `#F5F2E8` | Every outline and divider |
| `input` | `#000000` | `#F5F2E8` | Outline of fields, checkboxes, radios, slider |
| `ring` | `#2D5BFF` | `#7A9BFF` | Focus ring |
| `grid` | `#0000001A` | `#F5F2E81A` | The 24px grid behind a page (`blok-grid`) |

Shadows are tokens too and reference `foreground`, so they flip with the mode: `--shadow-xs` is `4px 4px 0 0 var(--foreground)` (controls), `--shadow-sm` is `6px 6px 0 0` (cards), `--shadow-lg` is `10px 10px 0 0` (menus, dialogs, toasts). Dark mode is the `.dark` class on a parent element: the ground turns near-black and the ink, outlines and shadows turn off-white; the five fills stay as they are.

Rules:

- Yellow is the primary action. One primary button per view; the yellow also marks the on state of controls and fills the marquee. Yellow is never text, and text on yellow is always black.
- Pink, blue and mint are fills for blocks, chips, card headers and stickers, never for text and never gradients. Each has one text color: black on pink and mint, white on blue.
- `foreground` does triple duty as text, outline and shadow. Do not introduce a gray outline or a gray shadow.
- Inverted blocks (`bg-foreground text-background`) are for selected chips, selected tabs, the "sold out" badge and the step that is done.
- Status colors are fills with words, never color alone.

Measured contrast (WCAG 2, both modes pass AA for text; most pass AAA):

| Pair | Light | Dark |
| --- | --- | --- |
| `foreground` on `background` | 20.7:1 | 16.7:1 |
| `foreground` on `card` | 21.0:1 | 15.4:1 |
| `foreground` on `secondary` | 18.1:1 | 12.8:1 |
| `primary-foreground` on `primary` | 16.6:1 | 16.6:1 |
| `primary-foreground` on `primary-hover` | 14.8:1 | 14.8:1 |
| `muted-foreground` on `background` | 7.7:1 | 9.0:1 |
| `muted-foreground` on `card` | 7.8:1 | 8.3:1 |
| `muted-foreground` on `secondary` | 6.7:1 | 6.9:1 |
| `background` on `foreground` (inverted blocks) | 21.0:1 | 18.8:1 |
| `pink-foreground` on `pink` | 7.4:1 | 7.4:1 |
| `blue-foreground` on `blue` | 5.2:1 | 5.2:1 |
| `mint-foreground` on `mint` | 14.2:1 | 14.2:1 |
| `destructive-foreground` on `destructive` | 5.0:1 | 5.0:1 |
| `success-foreground` on `success` | 9.4:1 | 9.4:1 |
| `warning-foreground` on `warning` | 8.9:1 | 8.9:1 |
| `input` outline against `card` | 21.0:1 | 15.4:1 |
| `ring` against `background` | 5.1:1 | 7.1:1 |

Two pairs fail and are therefore not allowed: black on `blue` is 4.1:1 (blue takes white text) and white on `pink` is 2.9:1 (pink takes black text). Yellow on white is 1.1:1, which is why yellow is never text.

## Typography

Archivo, the variable font with the width axis, and Space Mono, loaded by the app (Google Fonts, `@fontsource-variable/archivo` with the `wdth` axis, or `next/font` with `axes: ["wdth"]`). Archivo weights 400 to 900; Space Mono 400 and 700.

| Utility | Size / line | Weight | Tracking | Use |
| --- | --- | --- | --- | --- |
| `type-display` | 80 / 80 | 900, width 125 | -0.02em | The wordmark and the poster headline, one per page |
| `type-h1` | 56 / 56 | 800, width 125 | -0.02em | Page title |
| `type-h2` | 40 / 44 | 800, width 125 | -0.015em | Section title, the header wordmark |
| `type-h3` | 28 / 32 | 800, width 125 | -0.01em | Subsection, prices, the marquee, big stickers |
| `type-title` | 20 / 24 | 700 | 0 | Card and dialog titles |
| `type-body` | 16 / 24 | 400 | 0 | Body text, text inputs |
| `type-ui` | 14 / 20 | 600 | 0 | Field labels, options, chips, tabs, list rows, small buttons |
| `type-small` | 14 / 20 | 400 | 0 | Hints, secondary text, option labels |
| `type-caption` | 12 / 16, Space Mono | 400 | 0.02em | Captions, dates, metadata |
| `type-label` | 12 / 16, Space Mono, capitals | 700 | 0.08em | Badges, tags, card headers, step numbers, stickers |
| `type-mono` | 14 / 20, Space Mono | 400 | 0 | Times, prices, counts, code |

Buttons use `text-base font-bold` (16 / 24, weight 700).

Rules:

- Use the `type-*` utilities instead of composing size, weight, width and tracking by hand. They are not named `text-*` so that `tailwind-merge` does not confuse them with text colors.
- Display and headings are Archivo at width 125 (`font-stretch: 125%`) and weight 800 or 900. Body and interface text are the normal width. Never fake the width with a transform.
- Capitals are for the wordmark, the marquee, big stickers and `type-label`. Everything else is sentence case.
- Figures that line up (times, prices, counts) are `type-mono`.
- Text inputs stay at 16px so mobile browsers do not zoom on focus.

## Layout

- Spacing uses the Tailwind 4px unit and lands on an 8px grid: 8 inside a control, 16 between stacked options and as field padding, 24 as card padding and page margin, 32 between cards (the shadow takes 6 of it), 48 and 96 between sections. 12 and 20 appear only inside a control or a compact card.
- The page is `bg-background blok-grid`: the 24px grid shows between blocks. Cards sit on it with a 32px gap; do not place loose text on the grid except headlines and the marquee.
- Cards form a grid: one column on phones, two from 560px, three from 1024px, four from 1280px. A card is a column with a colored header bar and a body; it has no fixed ratio and is at least 336px tall in a gallery.
- The header is a `bg-card` bar with a 3px bottom border; the wordmark sits left and the theme switch is a 48px block on the right. Filters are a row of chips with a 12px gap that scrolls on small screens.
- Controls are 48px tall by default (buttons, fields, icon buttons, the theme switch); chips are 40, tabs 48 with their frame, badges 28, small icon buttons 32.

## Elevation & Depth

Depth is drawn, not lit. Every surface is flat; what makes a block a block is its outline and a hard shadow with no blur, offset down and right, in the outline color.

- `shadow-xs` (4px) on controls: buttons, icon buttons, chips, fields, toggles, checkboxes, the slider thumb, lists, tab frames, stickers, callouts.
- `shadow-sm` (6px) on cards and on a lifted control.
- `shadow-lg` (10px) on surfaces that float: menus, dialogs, toasts.
- `blok-press` gives a control its physics: hover moves it 2px up and left and grows the shadow to 6px; press, and `aria-pressed="true"`, move it 4px down and right and remove the shadow, so it sits where its shadow was. Disabled controls lose the shadow and drop to 40% opacity.
- Never a blurred shadow, a glow, a gradient or a translucent surface.

## Shapes

Nothing is round, with one exception.

- `--radius` is `0px` and every `rounded-*` class resolves to 0, so shadcn/ui components come out square.
- Outlines are 2px on controls and 3px on cards, marquees and big stickers. Dividers are 2px (`divide-y-2`).
- The radio is the one circle, so it reads as a radio next to the square checkbox.
- Stickers rotate by 3 to 6 degrees, either way. Nothing else is rotated.

Icons are Lucide at 16px (`size-4`) in `currentColor`, 20px when the icon stands alone in a 48px button or a callout. Icon-only buttons need an `aria-label`.

## Components

Copy these recipes. The live versions are in `preview/index.html`. Every block carries the same three parts: a 2px outline (`border-2 border-border`, 3px on cards), a hard shadow (`shadow-xs` on controls, `shadow-sm` on cards, `shadow-lg` on floating surfaces) and, when it can be clicked, `blok-press`.

### Button

48px block, 2px outline, 4px shadow, bold 16px text. One primary button per view.

```html
<button type="button" class="inline-flex h-12 items-center justify-center gap-2 border-2 border-border px-6 text-base font-bold shadow-xs blok-press disabled:pointer-events-none disabled:opacity-40 disabled:shadow-none bg-primary text-primary-foreground hover:bg-primary-hover">Get tickets<!-- 16px Lucide arrow-right --></button>
```

- Secondary: `bg-secondary text-secondary-foreground` instead of the primary colors.
- Outline: `bg-card text-foreground hover:bg-accent`.
- Small (40px): `h-10 px-4 type-ui` instead of `h-12 px-6 text-base font-bold`.
- Full width in a card: add `w-full`.

### Icon button

48px square block around a 20px icon. Inside a card header use `size-8` with a 16px icon.

```html
<button type="button" aria-label="Share" class="inline-flex size-12 items-center justify-center border-2 border-border bg-card text-foreground shadow-xs blok-press hover:bg-accent"><!-- 20px Lucide icon --></button>
```

For the one primary icon action use `bg-primary text-primary-foreground hover:bg-primary-hover`.

### Chip

40px filter block. Exactly one chip in a group has `aria-pressed="true"`; it is inverted and sits pressed into its shadow.

```html
<div role="group" aria-label="Programme" class="flex flex-wrap justify-center gap-3"><button type="button" aria-pressed="true" class="h-10 shrink-0 border-2 border-border bg-card px-4 type-ui text-foreground shadow-xs blok-press hover:bg-accent aria-pressed:bg-foreground aria-pressed:text-background">All</button><button type="button" aria-pressed="false" class="h-10 shrink-0 border-2 border-border bg-card px-4 type-ui text-foreground shadow-xs blok-press hover:bg-accent aria-pressed:bg-foreground aria-pressed:text-background">Riso</button></div>
```

### Toggle

56 by 32px block with a 24px square thumb. Checked, the track turns yellow and the thumb moves right. Flip `aria-checked` on click.

```html
<div class="flex items-center gap-4"><button type="button" role="switch" aria-checked="true" aria-labelledby="reminders" class="group relative h-8 w-14 shrink-0 border-2 border-border bg-card shadow-xs blok-press aria-checked:bg-primary disabled:opacity-40 disabled:shadow-none"><span class="absolute top-0.5 left-0.5 size-6 bg-foreground transition-transform group-aria-checked:translate-x-6"></span></button><span id="reminders" class="type-ui">Email reminders</span></div>
```

### Slider

A native range input with the `blok-slider` utility from `blok.css`: a 16px outlined track filled with yellow and a 24px block thumb. Chrome and Safari need `--slider-fill` to paint the filled part, so update it on every `input` event, and write the value into the `output`.

```html
<label class="block w-full"><span class="flex items-baseline justify-between"><span class="type-ui">Print run</span><output class="type-mono">120 copies</output></span><input type="range" min="20" max="500" step="10" value="120" data-unit="copies" class="mt-3 blok-slider" /></label>
```

```js
el.style.setProperty('--slider-fill', `${((el.value - el.min) / (el.max - el.min)) * 100}%`);
```

### Single selection (radio)

Native radios with the `blok-radio` utility, in a `fieldset` with a `legend`. The checked state is a 7px black ring around a yellow center. A figure on the right is `type-mono`.

```html
<fieldset class="flex w-full flex-col gap-4"><legend class="mb-4 type-ui">Pass</legend><label class="flex w-full items-center gap-3 type-small"><input type="radio" name="pass" checked class="blok-radio" />Day pass<span class="ml-auto type-mono text-muted-foreground">Rp50.000</span></label><label class="flex w-full items-center gap-3 type-small"><input type="radio" name="pass" class="blok-radio" />Weekend pass<span class="ml-auto type-mono text-muted-foreground">Rp120.000</span></label></fieldset>
```

### Checkbox

Native checkbox with the `blok-checkbox` utility: a 24px block with a 4px shadow; checked, it fills yellow with a black check.

```html
<fieldset class="flex w-full flex-col gap-4"><legend class="mb-4 type-ui">Add-ons</legend><label class="flex w-full items-center gap-3 type-small"><input type="checkbox" checked class="blok-checkbox" />Workshop seat</label><label class="flex w-full items-center gap-3 type-small"><input type="checkbox" class="blok-checkbox" />Printed programme</label></fieldset>
```

### Text field

48px block with a visible label above and a Space Mono hint below.

```html
<label class="block w-full"><span class="type-ui">Email</span><input type="email" placeholder="you@studio.id" class="mt-2 h-12 w-full border-2 border-input bg-card px-4 text-base shadow-xs placeholder:text-muted-foreground disabled:opacity-40 disabled:shadow-none" /><span class="mt-3 block type-caption text-muted-foreground">Your ticket is sent here.</span></label>
```

For an error, add `aria-invalid="true"`, swap `border-input` for `border-destructive`, and put the message in `type-caption text-destructive` below, saying how to fix the value.

### Tabs

One outlined block with 2px dividers; the selected tab is inverted. Arrow keys move the selection.

```html
<div role="tablist" aria-label="Day" class="inline-flex divide-x-2 divide-border border-2 border-border bg-card shadow-xs"><button type="button" role="tab" aria-selected="true" class="h-11 px-5 type-ui text-foreground transition-colors hover:bg-accent aria-selected:bg-foreground aria-selected:text-background">Fri</button><button type="button" role="tab" aria-selected="false" class="h-11 px-5 type-ui text-foreground transition-colors hover:bg-accent aria-selected:bg-foreground aria-selected:text-background">Sat</button></div>
```

### Badge

28px outlined tag in Space Mono capitals. The fill says the kind: mint for free, pink for new, warning for scarce, inverted for sold out. The word carries the meaning, not the color.

```html
<span class="inline-flex h-7 items-center border-2 border-border px-2.5 type-label bg-mint text-mint-foreground">Free</span>
```

### Progress

A 20px outlined track; the yellow fill ends in a 2px line. Write the figure next to the label.

```html
<div class="w-full"><div class="flex items-baseline justify-between"><span class="type-ui">Booths taken</span><span class="type-mono">64 / 80</span></div><div role="progressbar" aria-label="Booths taken" aria-valuenow="64" aria-valuemin="0" aria-valuemax="80" class="mt-2 h-5 w-full border-2 border-border bg-card"><div class="h-full w-[80%] border-r-2 border-border bg-primary"></div></div></div>
```

### List

An outlined block with 2px dividers. Rows hold a Space Mono figure, a title and, when needed, a `type-label` tag on the right.

```html
<ul class="w-full divide-y-2 divide-border border-2 border-border bg-card shadow-xs"><li class="flex items-center gap-4 px-4 py-3"><span class="type-mono text-muted-foreground">10:00</span><span class="type-ui">Doors open</span></li><li class="flex items-center gap-4 px-4 py-3"><span class="type-mono text-muted-foreground">11:00</span><span class="type-ui">Riso 101</span><span class="ml-auto type-label">Hall A</span></li></ul>
```

### Spinner

A 32px outlined square with a yellow top edge, turning in eight steps a second. It keeps turning under `prefers-reduced-motion`, since it reports progress; the steps keep the motion small.

```html
<span role="status" aria-label="Loading" class="block size-8 animate-step-spin border-3 border-border border-t-primary"></span>
```

### Card

3px outline, 6px shadow, a colored header bar with a `type-label` title and a body with 20px padding.

```html
<article class="flex w-full max-w-xs flex-col border-3 border-border bg-card shadow-sm"><header class="flex items-center justify-between gap-3 border-b-3 border-border bg-blue px-4 py-3 text-blue-foreground"><h3 class="type-label">Workshop</h3><span class="type-caption">Sat 21 · 11:00</span></header><div class="flex flex-col gap-3 p-5"><p class="type-title">Riso 101</p><p class="type-small text-muted-foreground">Two colours in one afternoon. Paper and ink are included; bring a sketch.</p><div class="flex items-center justify-between pt-1"><span class="type-mono">12 seats left</span><button type="button" class="h-10 border-2 border-border bg-card px-4 type-ui shadow-xs blok-press hover:bg-accent">Book</button></div></div></article>
```

The header color names the kind of content (yellow for actions, pink for input, blue for navigation, mint for feedback, inverted for content in the gallery); pick one mapping per product and keep it.

### Marquee

A strip with 3px rules, top and bottom, whose items scroll left for 28 seconds per loop. The list is doubled so the loop is seamless, and hidden from assistive technology; the sentence is in a visually hidden paragraph. It pauses on hover and stops under `prefers-reduced-motion`.

```html
<div class="w-full overflow-hidden border-y-3 border-border bg-primary py-3 text-primary-foreground"><p class="sr-only">Pasar Cetak, 20 to 22 November 2026, Bandung. Tickets on sale.</p><ul aria-hidden="true" class="flex w-max animate-marquee motion-reduce:animate-none hover:[animation-play-state:paused]"><li class="flex items-center gap-6 pr-6 type-h3 whitespace-nowrap uppercase">Pasar Cetak<span class="size-3 bg-foreground"></span></li><li class="flex items-center gap-6 pr-6 type-h3 whitespace-nowrap uppercase">20–22 Nov 2026<span class="size-3 bg-foreground"></span></li><!-- the same items once more --></ul></div>
```

An inverted strip is `bg-foreground text-background` with `bg-background` squares; add `[animation-direction:reverse]` to run it the other way.

### Accordion

Native `details` in an outlined block with 2px dividers. The yellow square shows + when closed and − when open.

```html
<div class="w-full divide-y-2 divide-border border-2 border-border bg-card shadow-xs"><details class="group" open><summary class="flex cursor-pointer list-none items-center justify-between gap-4 px-4 py-3 type-ui [&::-webkit-details-marker]:hidden">Can I bring my own paper?<span class="flex size-6 shrink-0 items-center justify-center border-2 border-border bg-primary text-primary-foreground [&>svg:first-child]:group-open:hidden [&>svg:last-child]:hidden [&>svg:last-child]:group-open:block"><!-- 16px Lucide plus --><!-- 16px Lucide minus --></span></summary><p class="px-4 pb-4 type-small text-muted-foreground">Yes, up to A3 and 300 gsm. Coated paper does not take riso ink well.</p></details></div>
```

### Steps

An ordered list with 32px numbered blocks joined by a 2px line. Done steps are inverted, the current step is yellow and carries `aria-current="step"`, steps to come are outlined.

```html
<ol class="flex w-full flex-col"><li class="relative flex gap-4 pb-6 before:absolute before:top-8 before:bottom-0 before:left-[15px] before:w-0.5 before:bg-border last:pb-0 last:before:hidden"><span class="flex size-8 shrink-0 items-center justify-center border-2 border-border type-label bg-foreground text-background" aria-hidden="true">1</span><div><p class="type-ui">Pick a pass</p><p class="type-caption text-muted-foreground">Weekend pass</p></div></li><li class="relative flex gap-4 pb-6 before:absolute before:top-8 before:bottom-0 before:left-[15px] before:w-0.5 before:bg-border last:pb-0 last:before:hidden" aria-current="step"><span class="flex size-8 shrink-0 items-center justify-center border-2 border-border type-label bg-primary text-primary-foreground" aria-hidden="true">2</span><div><p class="type-ui">Choose a workshop</p><p class="type-caption text-muted-foreground">Riso 101, 12 seats left</p></div></li></ol>
```

### Pricing tier

A card with a mint header, the price in `type-h3`, a list with square bullets and a full-width primary button. A sticker on the corner marks the recommended tier.

```html
<article class="relative flex w-full max-w-xs flex-col border-3 border-border bg-card shadow-sm"><span class="absolute -top-4 -right-3 rotate-6 inline-block border-2 border-border px-3 py-1.5 type-label whitespace-nowrap shadow-xs bg-pink text-pink-foreground">Best value</span><header class="border-b-3 border-border bg-mint px-5 py-3 text-mint-foreground"><h3 class="type-label">Weekend pass</h3></header><div class="flex flex-col gap-4 p-5"><p class="flex flex-wrap items-baseline gap-x-2"><span class="type-h3 whitespace-nowrap">Rp120.000</span><span class="type-caption text-muted-foreground">3 days</span></p><ul class="flex flex-col gap-2 type-small"><li class="flex items-center gap-3"><span class="size-2 shrink-0 bg-foreground"></span>Friday to Sunday</li><li class="flex items-center gap-3"><span class="size-2 shrink-0 bg-foreground"></span>One workshop seat</li></ul><button type="button" class="inline-flex h-12 items-center justify-center gap-2 border-2 border-border px-6 text-base font-bold shadow-xs blok-press disabled:pointer-events-none disabled:opacity-40 disabled:shadow-none w-full bg-primary text-primary-foreground hover:bg-primary-hover">Choose</button></div></article>
```

### Sticker

A rotated label block, 3 to 6 degrees either way. Small stickers are `type-label` on pink or mint; a big one is `type-h3` in capitals, inverted, with a 3px outline and the card shadow.

```html
<span class="-rotate-3 inline-block border-2 border-border px-3 py-1.5 type-label whitespace-nowrap shadow-xs bg-pink text-pink-foreground">Early bird</span>
```

```html
<span class="inline-block -rotate-6 border-3 border-border bg-foreground px-4 py-2 type-h3 whitespace-nowrap text-background uppercase shadow-sm">Sold out</span>
```

### Callout

A full-width note block with a 20px icon, a `type-ui` title and a `type-small` sentence. Mint for information, `bg-warning text-warning-foreground` with the triangle-alert icon for a warning.

```html
<div role="note" class="flex w-full items-start gap-3 border-2 border-border bg-mint p-4 text-mint-foreground shadow-xs"><span class="mt-0.5 shrink-0"><!-- 20px Lucide info --></span><div class="flex flex-col gap-1"><p class="type-ui">Doors open at 10:00</p><p class="type-small">The hall closes at 21:00 on Saturday. The last workshop starts at 18:00.</p></div></div>
```

### Newsletter

A field and a yellow button joined into one block that shares one shadow; the button has no left outline. The label is visible and a `type-caption` line says how often mail arrives.

```html
<form class="flex w-full flex-col gap-3"><label for="newsletter-email" class="type-ui">Get the schedule by email</label><div class="flex shadow-xs"><input id="newsletter-email" type="email" placeholder="you@studio.id" class="h-12 min-w-0 flex-1 border-2 border-input bg-card px-4 text-base placeholder:text-muted-foreground" /><button type="submit" class="h-12 shrink-0 border-2 border-l-0 border-border bg-primary px-5 text-base font-bold text-primary-foreground transition-colors hover:bg-primary-hover">Join</button></div><p class="type-caption text-muted-foreground">One email a week until the fair.</p></form>
```

### Toast

A floating block with the 10px shadow and an 8px colored stripe on the left. The action sits under the text so the toast fits a narrow column; the dismiss button is a quiet icon button.

```html
<div role="status" class="flex w-full max-w-sm items-start gap-3 border-2 border-l-8 border-border border-l-mint bg-card py-3 pr-2 pl-4 shadow-lg"><div class="flex min-w-0 flex-1 flex-col items-start gap-1"><p class="type-ui">Added to your order</p><p class="type-caption text-muted-foreground">2 × Weekend pass · Rp240.000</p><button type="button" class="mt-2 h-9 border-2 border-border bg-card px-3 type-ui shadow-xs blok-press hover:bg-accent">Undo</button></div><button type="button" data-dismiss aria-label="Dismiss" class="inline-flex size-9 shrink-0 items-center justify-center text-foreground hover:bg-accent"><!-- 16px Lucide x --></button></div>
```

### Focus

Every interactive element gets the global focus ring from `blok.css`: a 3px `ring` outline (cobalt in light mode, a lighter blue in dark mode) with a 2px offset. It is the only blue line in the system that is not a fill. Do not remove it.

## Do's and Don'ts

- Do give every block the same three parts: a 2px outline, a hard shadow in `foreground`, and `blok-press` when it can be clicked.
- Do keep one primary button per view. A second action is secondary or outline.
- Do set display and headings in Archivo at width 125 and weight 800 or 900, and labels in Space Mono capitals.
- Do pair every fill with its own text color: black on yellow, pink and mint; white on blue.
- Do give icon-only buttons an `aria-label` and form controls a visible label.
- Don't blur a shadow, add a gradient, a glow or a translucent surface. Depth is an offset in the outline color.
- Don't round a corner. The radio is the only circle.
- Don't use yellow, pink, blue or mint as text, or more than one loud fill on a single control.
- Don't use the default Tailwind palette or hard-coded hex values in components.
- Don't shrink interface text below 12px or text inputs below 16px, and don't fake the expanded width with a transform.
