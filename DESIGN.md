# Nicolas Portfolio Design System

## Intent

Single-page executive portfolio for international project leadership. The surface should feel calm, editorial, and business-focused: warm off-white paper, crisp dark typography, restrained accent colors, and quiet card depth.

## Tokens

- Ink: `#11151c`
- Muted text: `#5d6675`
- Paper: `#f5f6f2`
- Panel: `#ffffff`
- Line: `#d9dde3`
- Teal accent: `#0d6b70`
- Brick accent: `#93423f`
- Gold active marker: `#b48834`
- Radius: `8px`
- Primary shadow: `0 18px 60px rgba(17, 21, 28, 0.12)`

## Typography

- Font stack: Inter, system UI, Segoe UI, sans-serif.
- Body rhythm: 1.55 line-height for readability across English and Japanese.
- Section kicker: `0.78rem`, uppercase/label style.
- Hero display heading: `clamp(1.89rem, 4.9vw, 4.34rem)`, reduced 30% from the original hero scale.
- Hero display heading on mobile: `clamp(1.68rem, 8.06vw, 2.41rem)`.
- Mobile hero heading line length is capped at `8.8em` with natural word wrapping to preserve readable lines.
- Mobile hero intro copy is capped at `22em` to prevent edge-hugging lines.
- Section heading: `clamp(1.4rem, 3.08vw, 2.8rem)`, reduced 30% from the original section scale.
- Section heading on mobile: `clamp(1.82rem, 4vw, 3.64rem)`.
- Section body copy: `1.08rem`, matching the About Me body standard.
- Section body line-height: `1.62`.
- Section card title: `1.22rem`, with larger local variants only where hierarchy requires it.
- Section metadata: `0.94rem`.
- Section label/kicker: `0.78rem`.
- Section paragraph gap: `18px`.
- Section card internal gap: `14px`.
- Display hero heading is intentionally separate from section typography, but should remain quieter than the first prototype scale.
- No negative letter spacing.

## Layout

- Desktop uses a sticky 292px sidebar and single scrolling content column.
- Mobile collapses to a top identity/navigation bar and single-column content.
- Sections are full-width content bands with constrained inner content; cards are reserved for repeated records and framed portfolio items.

## Components

- Sidebar identity: portrait, name, subtitle, current section, nav links, footer contact.
- Language switch: desktop uses a compact segmented control in the sidebar; narrow layouts use a small flag button as the first navigation item before About Me, styled with the same soft capsule language as the nav.
- Timeline item: two-column desktop card with date rail and role body, collapsing to one column on mobile.
- Project card: image/media header, category label, title, summary, metadata chips, link.
- Chips/tags: non-clickable metadata treatments; links remain visually distinct as underlined or bordered actions.

## Motion

- Hero background images crossfade every 6 seconds using opacity only.
- Honor `prefers-reduced-motion` by disabling the automatic hero carousel.
