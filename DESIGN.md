---
name: Pixel Blossom
colors:
  surface: '#fff7f9'
  surface-dim: '#fecbef'
  surface-bright: '#fff7f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#ffeff7'
  surface-container: '#ffe7f5'
  surface-container-high: '#ffdff4'
  surface-container-highest: '#ffd7f2'
  on-surface: '#2f0f2b'
  on-surface-variant: '#53424c'
  inverse-surface: '#472441'
  inverse-on-surface: '#ffebf6'
  outline: '#86717c'
  outline-variant: '#d8c0cc'
  surface-tint: '#a02f85'
  primary: '#a02f85'
  on-primary: '#ffffff'
  primary-container: '#fe7fd8'
  on-primary-container: '#7a0364'
  inverse-primary: '#ffade1'
  secondary: '#6d5e00'
  on-secondary: '#ffffff'
  secondary-container: '#ffe252'
  on-secondary-container: '#746400'
  tertiary: '#944a00'
  on-tertiary: '#ffffff'
  tertiary-container: '#fa923c'
  on-tertiary-container: '#673200'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffd8ed'
  primary-fixed-dim: '#ffade1'
  on-primary-fixed: '#3b002f'
  on-primary-fixed-variant: '#83106b'
  secondary-fixed: '#ffe252'
  secondary-fixed-dim: '#e1c638'
  on-secondary-fixed: '#211b00'
  on-secondary-fixed-variant: '#524600'
  tertiary-fixed: '#ffdcc5'
  tertiary-fixed-dim: '#ffb784'
  on-tertiary-fixed: '#301400'
  on-tertiary-fixed-variant: '#713700'
  background: '#fff7f9'
  on-background: '#2f0f2b'
  surface-variant: '#ffd7f2'
  background-gradient-start: '#A22CE4'
  background-gradient-end: '#A689F3'
  surface-navigation: '#F3E2E8'
  plum-outline: '#43213D'
  text-on-accent: '#43213D'
typography:
  display-hero:
    fontFamily: Press Start 2P
    fontSize: 3rem
    fontWeight: '700'
    lineHeight: 3.5rem
    letterSpacing: 0px
  display-hero-mobile:
    fontFamily: Press Start 2P
    fontSize: 1.5rem
    fontWeight: '700'
    lineHeight: 2rem
    letterSpacing: 0px
  headline-md:
    fontFamily: Press Start 2P
    fontSize: 1rem
    fontWeight: '700'
    lineHeight: 1.5rem
    letterSpacing: 0px
  body-default:
    fontFamily: Courier Prime
    fontSize: 0.875rem
    fontWeight: '700'
    lineHeight: 1.375rem
  body-sm:
    fontFamily: Courier Prime
    fontSize: 0.75rem
    fontWeight: '400'
    lineHeight: 1.125rem
  label-badge:
    fontFamily: Press Start 2P
    fontSize: 0.625rem
    fontWeight: '700'
    lineHeight: 0.875rem
    letterSpacing: 0.05em
  label-nav:
    fontFamily: Courier Prime
    fontSize: 0.875rem
    fontWeight: '700'
    lineHeight: 1rem
  button-text:
    fontFamily: Press Start 2P
    fontSize: 0.6875rem
    fontWeight: '700'
    lineHeight: 1rem
spacing:
  gutter: 0.75rem
  margin: 1rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 3.625rem
---

## Brand & Style

This design system establishes a warm, nostalgic, and enchanting aesthetic tailored for a cozy fantasy pixel-art game experience. It balances playful retro 16-bit arcade sentiment with a disciplined neubrutalist framing structure. 

The emotional signature is whimsical, comforting, and direct. The interface intentionally evokes early PC RPG and cartridge console game interfaces while maintaining modern web responsiveness. Visual hierarchy is established not through soft blurs or modern ambient drop-shadows, but through intentional pixel-grid framing, high-contrast flat planes, saturated pastel accents, and rigid dark-plum outlines.

## Colors

The system uses a saturated vertical gradient background transitioning from bold electric purple (`#A22CE4`) at the canvas top down into soft lavender (`#A689F3`). 

Structural surfaces use a delicate pale blush (`#F3E2E8`), creating high tonal contrast against the background while harmonizing with the warm fantasy palette. 

- **Primary (`#FE7FD8`)**: Vibrant cherry blossom pink used for primary calls to action (Download CTA) and key categorization tags.
- **Secondary (`#F5D94A`)**: Sunflower yellow used for carousel navigation controls and secondary activity chips.
- **Tertiary (`#F28B36`)**: Warm marigold orange reserved for tertiary genre classifications and supplemental badges.
- **Neutral / Outlines (`#43213D`)**: Deep roasted plum utilized as the sole structural stroke, text color, and border tone. Pure black is never used; dark plum anchors the palette with retro warmth.

## Typography

Typography prioritizes authentic pixelated hardware aesthetics paired with legible retro-computing forms.

- **Display & Labels**: Driven by `Press Start 2P`. Used strictly for the main brand title, genre tag chips, gallery navigation controls, and CTA buttons. Monospaced character grids must align squarely without arbitrary letter-spacing.
- **Body & Navigation Links**: Driven by `Courier Prime` (or `Courier New` fallbacks). Used for navigational items, secondary headers, narrative subheadings, and descriptive captions.
- **Casing Rules**: Subtitles, game categories, and primary buttons must always render in uppercase (`text-transform: uppercase`).

## Layout & Spacing

The layout is built around a centralized single-column stage with a fixed maximum desktop width of `824px`. 

- **Outer Rhythm**: The canvas utilizes generous vertical padding (`3.625rem` / `58px`) above the navigation bar, and an identical `58px` vertical interval isolating the navigation bar from the hero showcase frame.
- **Gallery Cadence**: The hero frame sits immediately above a four-item thumbnail gallery linked by a tight `10px` to `12px` vertical gap.
- **Responsive Stacking**: On tablet and mobile viewports, the `824px` content container fluidly scales to `calc(100vw - 2rem)`. The navigation bar transitions gracefully from horizontal inline flex to a centered stack or compact bar while preserving horizontal button alignment. The hero scene maintains an intrinsic `16:9` aspect ratio.

## Elevation & Depth

This system rejects ambient blurs, fuzzy dropshadows, glassmorphic filters, and elevation gradients. Visual separation and layering are achieved through strictly planar methods:

- **Border Enclosures**: All interactive containers, frames, and buttons are outlined with a crisp `2px solid #43213D` stroke.
- **Physical Hard Offsets**: Active components or elevated frames achieve tactile depth using a hard, unblurred retro offset shadow (`box-shadow: 2px 2px 0px #43213D` or `3px 3px 0px #43213D`).
- **Active States**: Focused or active items (such as the active gallery thumbnail) receive an amplified `3px solid #43213D` border to signify focus without expanding element layout dimensions.

## Shapes

The geometric vocabulary is uncompromisingly sharp (`roundedness: 0`). 

- Major framing components—including the navigation container, hero viewport, and gallery frames—must have `border-radius: 0px`.
- Interactive chips and buttons use crisp `0px` corners, with small buttons optionally permitted a subtle `2px` radius (`rounded-xs`) only when softening contrast against high-density game graphics.
- Imagery must be rendered with `image-rendering: pixelated` to preserve hard pixel corners across high-DPI viewports.

## Components

### Navigation Bar
- Height: `54px`.
- Fill: Pale blush (`#F3E2E8`) enclosed by a `2px solid #43213D` border.
- Layout: Flexbox container featuring the pixel logo on the far left, centered textual navigation items (`News`, `Characters`, `Support`, `Terms & Privacy` in `Courier Prime`, dark plum), and the pink Download CTA aligned to the far right.

### Buttons
- **Download CTA**: Background `#FE7FD8`, border `2px solid #43213D`, text `#43213D` set in `Press Start 2P` (`11px`). Hover state applies an immediate `1px` downward-right transform with a matching hard pixel drop.
- **Carousel Controls (Previous / Next)**: Square `#F5D94A` boxes with `2px solid #43213D` framing, harboring black pixel-rendered chevron glyphs. Positioned over the mid-flanks of the hero container.

### Category Chips
- Compact horizontal tags pinned below the hero narrative.
- Standardized `2px solid #43213D` border, zero border-radius, uppercase text set in `label-badge` (`10px`).
- Tone assignments:
  - Exploration: Primary Pink (`#FE7FD8`)
  - Farming: Secondary Yellow (`#F5D94A`)
  - Life Sim: Tertiary Orange (`#F28B36`)

### Hero Showcase Frame
- Exact `16:9` ratio container (`824px × 464px` on desktop) bound with a `2px solid #43213D` frame.
- Overlaid with bottom-left positioned brand title in `display-hero` typography, accompanied by the two-line subtitle: `"A COZY ADVENTURE / IN A BRIGHTER WORLD"`.

### Thumbnail Gallery
- Horizontal 4-column grid spanning the full `824px` width of the hero container.
- Each thumbnail is an aspect-ratio-locked landscape image framed by a `2px solid #43213D` outline.
- **Active State**: The selected thumbnail applies an amplified `3px solid #43213D` outline and 100% opacity, while unselected thumbnails rest at `80%` opacity with a standard `2px` stroke.