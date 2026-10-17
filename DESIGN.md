---
name: Will & Cora — Save the Date
description: A frameless hand-painted save-the-date that dissolves into white paper and lends its own colours to a playful RSVP.
colors:
  ground-white: "#ffffff"
  ink-sepia: "#5a3621"
  ink-soft: "#786046"
  hairline: "#ebe3d7"
  line-strong: "#cfc8bb"
  river: "#19615c"
  river-deep: "#124a46"
  river-teal: "#2f8a79"
  sea-green: "#56aa91"
  hill-green: "#4a9540"
  hill-green-soft: "#639a5e"
  hill-green-deep: "#416930"
  olive: "#9c8a3e"
  roof-terracotta: "#af7447"
  pass-green: "#3f6a2f"
  fail-terracotta: "#9a5a37"
  button-ink: "#f6f3ea"
  gauge-unlaid: "#f1ede4"
typography:
  display:
    fontFamily: "Spectral, Georgia, 'Times New Roman', serif"
    fontSize: "clamp(2rem, 9vw, 2.8rem)"
    fontWeight: 500
    lineHeight: 1.08
    letterSpacing: "0.006em"
  question:
    fontFamily: "Spectral, Georgia, 'Times New Roman', serif"
    fontSize: "clamp(1.55rem, 5.8vw, 2.15rem)"
    fontWeight: 500
    lineHeight: 1.26
    letterSpacing: "0.006em"
  body:
    fontFamily: "Spectral, Georgia, 'Times New Roman', serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: "normal"
  button:
    fontFamily: "Spectral, Georgia, 'Times New Roman', serif"
    fontSize: "1.1rem"
    fontWeight: 500
    lineHeight: 1.6
    letterSpacing: "0.03em"
  label:
    fontFamily: "Spectral, Georgia, 'Times New Roman', serif"
    fontSize: "0.72rem"
    fontWeight: 600
    lineHeight: 1.6
    letterSpacing: "0.24em"
  signature:
    fontFamily: "Spectral, Georgia, 'Times New Roman', serif"
    fontSize: "0.66rem"
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: "0.05em"
rounded:
  xs: "1.5px"
  sm: "2px"
  md: "4px"
spacing:
  page-x: "22px"
  tile-gap: "3px"
  gauge-gap: "8px"
  yesno-gap: "18px"
components:
  button-primary:
    backgroundColor: "{colors.river}"
    textColor: "{colors.button-ink}"
    typography: "{typography.button}"
    rounded: "{rounded.md}"
    padding: "13px 44px"
  button-primary-hover:
    backgroundColor: "{colors.river-deep}"
    textColor: "{colors.button-ink}"
  button-ghost:
    backgroundColor: "{colors.ground-white}"
    textColor: "{colors.ink-sepia}"
    typography: "{typography.button}"
    rounded: "{rounded.md}"
    padding: "12px 34px"
  choice:
    backgroundColor: "transparent"
    textColor: "{colors.ink-sepia}"
    typography: "{typography.body}"
    rounded: "0"
    padding: "16px 8px 16px 6px"
  choice-hover:
    textColor: "{colors.river}"
    padding: "16px 8px 16px 18px"
  text-link:
    backgroundColor: "transparent"
    textColor: "{colors.river}"
    typography: "{typography.label}"
    padding: "0 0 3px"
  text-link-hover:
    textColor: "{colors.river-deep}"
---

# Design System: Will & Cora — Save the Date

## Overview

**Creative North Star: "The Painting, Continued"**

The page is the hand-painted save-the-date itself, continued past its own edges onto the white of the paper. The illustration sits frameless at the top — no border, no card, no shadow — on the exact white (#ffffff) the painter worked against, so the artwork and the page are one surface. Everything below is set in that same white and borrows its colour from nowhere but the painting: the teal of the river, the greens of the hills, the olive and terracotta of the roofs. There is no brand palette layered on top; the artwork is the palette.

The world is quiet, warm, and legible. Type is a single serif (Spectral) in a warm sepia ink that is deliberately never black, echoing the save-the-date's hand-lettering. Density is low and vertical: one narrow column, generous air, fluid type that scales with the viewport rather than snapping at breakpoints. The one loud gesture is the signature element — a CSS-grid mosaic of square tiles that reassembles the painting's colours into a single cresting wave, with the white page itself showing through the grout. Mischief (a "No" button that flees the cursor, a gauge that lays coloured pavers as you walk through the quiz) is carried by motion and colour, never by chrome.

This is a committed single light world: `color-scheme: light`, one ground, no theme toggle, no dark mode. The anti-reference is the polished vendor wedding template — nothing here should read as stock. Warmth and the hand are the point.

**Key Characteristics:**
- One white ground shared by the artwork and the page; the painting is frameless and dissolves into it.
- The painting's own colours are the entire colour system — no imported brand hues.
- Warm sepia ink, never black, for all text.
- A single serif (Spectral) throughout; the question and verdict are italic.
- A tile mosaic ("the wave") as the signature, grouted by the white page.
- Committed single light world; fluid type and spacing instead of hard breakpoints.

## Colors

A warm, painterly palette lifted wholesale from the hand-painted save-the-date: teals and greens from the river and hills, olive and terracotta from the roofs, all sitting on the painting's own white.

### Primary
- **River Teal** (#19615c): The deep teal of the river and the single primary action colour. It fills the "Yes" button, draws the focus ring and text selection, starts the progress gauge, and is the default hover tint for answer rows and the retry link.
- **River Deep** (#124a46): The pressed/hover darkening of River Teal — the "Yes" button and retry link deepen to it on interaction.

### Secondary
Painting greens and teal-greens — used structurally in the wave mosaic and as answer-row hover tints.
- **River Teal-Green** (#2f8a79): Mid teal-green wave tile.
- **Sea Green** (#56aa91): Light teal-green wave tile.
- **Hill Green** (#4a9540): The hills; second colour of the progress gauge and a wave tile.
- **Hill Green Soft** (#639a5e): Lighter hill tone in the wave.
- **Hill Green Deep** (#416930): Shadowed hill tone in the wave.

### Tertiary
Roof and earth tones — the warm end of the painting.
- **Olive** (#9c8a3e): Dry olive-gold roof tone; a wave tile and an answer-hover tint.
- **Roof Terracotta** (#af7447): The terracotta roof; the final colour of the progress gauge, a wave tile, and an answer-hover tint.

### Semantic (verdict)
- **Pass Green** (#3f6a2f): The "You passed!" verdict title only. A deeper, calmer green than the hill tiles.
- **Fail Terracotta** (#9a5a37): The "You're uninvited!" verdict title only. A deeper, earthier terracotta than the roof tile.

### Neutral
- **Ground White** (#ffffff): The single page background and the painting's own white — the two are the same surface. Also the grout showing between mosaic and gauge tiles.
- **Ink Sepia** (#5a3621): Warm sepia, the body and heading ink. The hand-lettering's colour.
- **Ink Soft** (#786046): Muted warm brown for secondary text — the verdict subtitle and the closing signature (holds AA).
- **Hairline** (#ebe3d7): Warm hairline rules between and around the answer list.
- **Line Strong** (#cfc8bb): Ghost-control edge — the resting border of the "No" button and unlaid gauge pavers.
- **Button Ink** (#f6f3ea): Warm off-white for text on the filled River Teal button — never pure white.
- **Gauge Unlaid** (#f1ede4): The fill of a gauge paver not yet walked past.

### Named Rules
**The Painting Is the Palette Rule.** Every colour in the system comes from the save-the-date illustration. Do not introduce a hue that is not already in the artwork; if a new surface needs a colour, take it from the painting's own range (teals, hills, olive, terracotta) rather than inventing one.

**The Never-Black Rule.** Text is warm sepia (#5a3621) or soft brown (#786046), never #000. White-on-colour text is warm off-white (#f6f3ea), never #fff. The whole ink range leans warm to match the hand-lettering.

**The One Action Rule.** River Teal (#19615c) is the only colour that means "do this." It is reserved for the primary action, focus, and selection. The greens, olive, and terracotta are decorative (the wave) or responsive tints (answer hover, gauge progress), not call-to-action colours.

## Typography

**Display / Body Font:** Spectral (with Georgia, "Times New Roman", serif fallback)

**Character:** One serif does everything. Spectral is a warm, slightly literary text serif; set in sepia it reads as hand-and-ink rather than system type. The emotional register comes entirely from italics — the question and the verdict are the only italic elements, and they carry the voice.

### Hierarchy
- **Display** (weight 500, italic, clamp(2rem, 9vw, 2.8rem), line-height 1.08): The verdict title ("You passed!" / "You're uninvited!"). Coloured by semantic pass/fail.
- **Question** (weight 500, italic, clamp(1.55rem, 5.8vw, 2.15rem), line-height 1.26, max-width 18ch, balanced): The gate question and each quiz question. Centred, in sepia ink.
- **Body** (weight 400, 16px, line-height 1.6): Base reading size. The verdict subtitle is a 1.05rem italic variant in Ink Soft (max-width 32ch); answer rows are a 1.12rem upright variant in sepia.
- **Button** (weight 500, 1.1rem, letter-spacing 0.03em): The "Yes" and "No" buttons.
- **Label** (weight 600, 0.72rem, letter-spacing 0.24em, uppercase): The retry link ("take it again" / "redeem yourself") — the only uppercase, wide-tracked text in the system.
- **Signature** (weight 400, 0.66rem, letter-spacing 0.05em): The closing footer line, with its riddle clause set italic. A pencil whisper at the foot of the page.

### Named Rules
**The Italic-Voice Rule.** Italics mark the two emotional beats only — the question being asked and the verdict being delivered. Everything else (answers, buttons, signature prose) is upright. Do not set body copy or UI labels in italic.

**The One-Serif Rule.** Spectral is the only typeface. No sans, no mono, no display face is introduced for contrast; hierarchy is built from size, weight, italic, and letter-spacing within the one family.

## Layout

A single centred column, max-width 560px, with fluid horizontal padding of 22px that respects the safe-area insets (`env(safe-area-inset-*)`), so the page is phone-first and never collides with a notch. Vertical rhythm is fluid rather than stepped: section gaps, the top/bottom page padding, and element margins are almost all `clamp()` expressions that scale with viewport width, so there are no hard breakpoints — the layout breathes continuously from phone to desktop. The painting spans the full column width at the top (max 100%); the wave mosaic is capped at 440px and the answer list at 430px, both centred, keeping interactive content slightly narrower than the artwork. Content advances by reveal, not by scroll regions: the gate, quiz, and verdict are stacked panels that show one at a time and smooth-scroll into centre view (honouring `prefers-reduced-motion`).

## Elevation & Depth

Nearly flat. The page has no cards, no raised surfaces, and no drop shadows around content — the painting is explicitly frameless and fused to the white ground. Depth appears in exactly two places and both are subtle and tactile, not elevation chrome: a soft colour-matched lift under the filled "Yes" button, and faint inset bevels on the small square tiles (mosaic and gauge) to read as hand-set ceramic rather than flat fills.

### Shadow Vocabulary
- **Action lift** (`box-shadow: 0 1px 2px rgba(18,74,70,.2), 0 10px 22px -12px rgba(18,74,70,.55)`): The resting shadow under the "Yes" button, tinted in the River Deep colour rather than neutral grey — a diffuse glow that belongs to the teal, not a generic elevation.
- **Tile bevel, laid** (`box-shadow: inset 0 1px 0 rgba(255,255,255,.28), inset 0 -1px 2px rgba(0,0,0,.08)`): Inset top-light / bottom-shade on a coloured mosaic tile and a laid gauge paver, giving each square a set-in-grout feel. The gauge paver uses a marginally stronger variant (`…rgba(255,255,255,.35)…rgba(0,0,0,.1)`).
- **Tile edge, unlaid/current** (`box-shadow: inset 0 0 0 1px #cfc8bb` resting; `inset 0 0 0 1.5px #5a3621` for the current step): A hairline inset ring that outlines a not-yet-walked gauge paver, thickening to sepia on the step you are on.

### Named Rules
**The Frameless Rule.** The artwork and content surfaces carry no border, card, or drop shadow. The only shadows in the system are the one tinted action lift and the inset tile bevels. Do not box content or add ambient card shadows.

## Shapes

Barely-rounded rectangles. The form language is near-square: tiles are 1.5px radius, gauge pavers and focus outlines 2px, buttons 4px. Nothing is pill-shaped or circular. The defining geometry is the grid of squares — the wave mosaic and the progress gauge are both built from small squares separated by white grout, and that tiled square is the recurring motif of the system. Rules are thin single hairlines (1px) between answer rows; the answer list is a ruled list, never a set of boxes or chips.

## Components

### Buttons
- **Shape:** Gently squared corners (4px radius).
- **Primary ("Yes"):** Filled River Teal (#19615c) with warm off-white ink (#f6f3ea), padding 13px 44px, carrying the tinted action-lift shadow. Hover deepens the fill to River Deep (#124a46) and lifts 1px (`translateY(-1px)`); active settles back to 0.
- **Ghost ("No"):** White background, sepia ink, 1px Line Strong (#cfc8bb) border, padding 12px 34px. Hover darkens the border to Ink Soft. This button is unclickable by design — on hover, focus, mouse-down, touch, or near-approach it switches to `position: fixed` and flees to a random spot with a small random rotation, dodging both cursor and finger. It can never be pressed.

### Choices (answer list)
- **Style:** A clean ruled list, not tiles or chips. Each answer is a full-width, left-aligned button with no background and no side borders, separated by 1px Hairline (#ebe3d7) rules (the list also has a top rule). Body serif at 1.12rem in sepia.
- **State:** On hover/focus the row tints its text and bottom rule to a per-row colour from the painting (teal → hill green → olive → terracotta, cycling) and nudges its left padding in from 6px to 18px — an approach, not a fill.

### Progress Gauge (signature)
- **Style:** A centred row of 14px squares (2px radius, 8px gaps), one per quiz question. An unlaid paver is Gauge Unlaid (#f1ede4) with a Line Strong inset hairline; the current step gets a sepia inset ring and scales up 1.16×; a walked step is "laid" — filled with one distinct wave colour per step (teal #19615c → hill green #4a9540 → terracotta #af7447) and given the inset tile bevel. A newly laid paver plays a 0.45s pop-in reveal. All motion is suppressed under `prefers-reduced-motion`.

### The Wave (signature)
- **Style:** A CSS-grid mosaic, max-width 440px, of 25×9 square tiles (1.5px radius, 3px gaps) generated in JS. Tiles lying along one full sine period are coloured from the eight-colour painting palette (#19615c, #2f8a79, #56aa91, #4a9540, #639a5e, #416930, #9c8a3e, #af7447) and carry the inset tile bevel; the rest stay empty so the white page shows through as grout, drawing a single cresting wave. Decorative and `aria-hidden`.

### Retry link
- **Style:** A borderless text button in uppercase Label type (0.72rem, letter-spacing 0.24em, weight 600) in River Teal with a 1px underline in the current colour. Hover deepens to River Deep. The system's only uppercase, wide-tracked element.

### Focus & Selection
- **Focus-visible:** 2px River Teal outline, 3px offset, 2px radius — the one global focus treatment.
- **Selection:** River Teal background with white text.

## Do's and Don'ts

### Do:
- **Do** take every colour from the save-the-date painting; pull new hues from its own teal/green/olive/terracotta range (The Painting Is the Palette Rule).
- **Do** set all text in warm sepia (#5a3621) or soft brown (#786046), and white-on-teal text in warm off-white (#f6f3ea), never pure black or white (The Never-Black Rule).
- **Do** reserve River Teal (#19615c) for the single primary action, focus, and selection; let greens/olive/terracotta stay decorative or responsive tints (The One Action Rule).
- **Do** build repeated colour moments as small grouted squares (the wave, the gauge) rather than bars or blocks.
- **Do** keep type in Spectral and scale hierarchy with `clamp()`, size, weight, italic, and tracking — not with a second typeface.
- **Do** use italics only for the question and the verdict (The Italic-Voice Rule).

### Don't:
- **Don't** frame, box, card, or drop-shadow the artwork or content surfaces; the only shadows are the tinted action lift and the inset tile bevels (The Frameless Rule).
- **Don't** introduce dark mode, a theme toggle, or any ground other than #ffffff — this is a committed single light world.
- **Don't** turn the answers into tiles, chips, or boxes; they are a hairline-ruled list that tints and shifts on approach.
- **Don't** add a sans-serif, monospace, or display typeface for contrast.
- **Don't** make the "No" button clickable or give it a confirmed resting place; its dodging on both mouse and touch is the gag.
