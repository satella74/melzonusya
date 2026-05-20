---
name: Joyful Pieces
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#40484f'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#707880'
  outline-variant: '#bfc7d0'
  surface-tint: '#006491'
  primary: '#006491'
  on-primary: '#ffffff'
  primary-container: '#7bc9ff'
  on-primary-container: '#00547a'
  inverse-primary: '#8aceff'
  secondary: '#9c4050'
  on-secondary: '#ffffff'
  secondary-container: '#fd8c9c'
  on-secondary-container: '#772334'
  tertiary: '#665e49'
  on-tertiary: '#ffffff'
  tertiary-container: '#ccc0a7'
  on-tertiary-container: '#564e3a'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#c9e6ff'
  primary-fixed-dim: '#8aceff'
  on-primary-fixed: '#001e2f'
  on-primary-fixed-variant: '#004c6e'
  secondary-fixed: '#ffd9dc'
  secondary-fixed-dim: '#ffb2bb'
  on-secondary-fixed: '#400011'
  on-secondary-fixed-variant: '#7e2839'
  tertiary-fixed: '#eee1c7'
  tertiary-fixed-dim: '#d1c5ac'
  on-tertiary-fixed: '#211b0b'
  on-tertiary-fixed-variant: '#4e4633'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  headline-lg:
    fontFamily: Quicksand
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Quicksand
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 34px
  headline-md:
    fontFamily: Quicksand
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  body-lg:
    fontFamily: Quicksand
    fontSize: 20px
    fontWeight: '500'
    lineHeight: 30px
  body-md:
    fontFamily: Quicksand
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 28px
  label-bold:
    fontFamily: Quicksand
    fontSize: 16px
    fontWeight: '700'
    lineHeight: 20px
rounded:
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 40px
  xl: 64px
  gutter: 20px
  margin-mobile: 16px
  margin-desktop: 48px
---

## Brand & Style

This design system is built to evoke a sense of wonder, safety, and boundless creativity. The target audience—young children and their parents—requires a UI that feels like a physical toy: tactile, forgiving, and high-energy.

The design style is **Modern Playful Minimalism**. It takes the clarity of a flat UI and softens every edge, removing all visual "sharpness." By combining generous white space with a vibrant, candy-toned palette, the interface remains uncluttered and easy for developing motor skills to navigate. The emotional response is one of "soft joy"—an inviting digital playground that feels modern rather than dated or cluttered.

## Colors

The palette is inspired by a sunny day at the park. 

- **Primary (Sky Blue):** Used for main actions, navigation headers, and "safe" interactions.
- **Secondary (Coral Pink):** Reserved for high-energy moments, "Win" states, and delightful surprises.
- **Tertiary (Soft Yellow):** The primary background tint for containers and cards to keep the UI warm and approachable.
- **Accent (Mint Green):** Specifically for "Correct" puzzle placements and progress indicators.
- **Neutral:** A very light, cool-toned white is used for the base canvas to ensure the soft colors pop without causing eye strain.

## Typography

We use **Quicksand** exclusively for its geometric, rounded terminals which mirror the shape of the UI components. 

Typography must be exceptionally legible. Font sizes are scaled up (minimum 18px for body) to ensure readability for young users. Headlines use a tight letter-spacing to feel "chunky" and impactful, while body text is given generous line height to prevent the UI from feeling cramped. All labels should avoid complex jargon, using simple, direct verbs.

## Layout & Spacing

The layout philosophy is based on **Breathable Containers**. We use a 12-column fluid grid for desktop and a 4-column grid for mobile, but with unusually large margins to keep interaction targets away from the screen edges.

Spacing follows an 8px rhythmic scale. However, for "Kid-Safe" zones, we prioritize `lg` (40px) and `xl` (64px) padding within cards to ensure puzzle pieces and buttons have plenty of "miss-click" room. On mobile, elements should reflow into a single-column stack with large, vertical gutters to prevent accidental taps on neighboring items.

## Elevation & Depth

To maintain a friendly aesthetic, we avoid harsh, realistic shadows. Depth is communicated through **Cloud Shadows**:

- **Low Elevation:** Use a soft, wide-spread shadow with 5% opacity of the Primary color (Sky Blue) rather than black. This makes elements feel like they are floating gently above the surface.
- **Active States:** When a user taps or drags a puzzle piece, the shadow should expand in blur radius and slightly increase in offset, simulating the piece being "picked up" closer to the user.
- **Inner Depth:** For "empty" puzzle slots, use a subtle inner-glow in a darker tint of the Tertiary color to create a "well" effect, signaling where pieces should be placed.

## Shapes

The shape language is strictly **Hyper-Rounded**. Every interactive element uses a pill-shape or a corner radius that is at least 50% of the element's height where possible. 

Avoid sharp 90-degree angles entirely. Even container backgrounds and selection overlays must utilize `rounded-xl` (1.5rem) settings. This visual softness reinforces the brand's safety and friendliness, making the digital environment feel "cushioned."

## Components

### Buttons
Buttons are "chunky" and high-contrast. Use a 4px bottom border (a slightly darker shade of the button color) to give a faux-3D "pressable" look. The Primary button uses Sky Blue, while "Back" or "Cancel" buttons use a soft grey-blue.

### Cards & Puzzle Slots
Cards are the white canvas for the puzzle. They feature a `md` (24px) internal padding and `rounded-xl` corners. Puzzle slots are dashed outlines with the same roundedness, using the Tertiary color for the stroke.

### Chips & Badges
Used for difficulty levels (Easy, Medium, Hard). These are full-pill shapes with white text. Use Mint Green for "Easy" and Coral Pink for "Hard."

### Progress Bars
Progress bars are thick (at least 20px height) with rounded caps. The track is the Tertiary color, and the fill is the Accent Mint Green.

### Input Fields
Since the target is kids, input fields are minimal. Use large, oversized text areas with a simple Sky Blue border. Icons should be used alongside labels to provide visual cues (e.g., a magnifying glass icon for "Search").

### Feedback Modals
Success messages should be large, centered overlays with a Coral Pink confetti-style border. Keep text to a maximum of three words (e.g., "Great Job, Scout!").