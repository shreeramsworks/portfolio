# Design System — Shreeram S. Kulkarni Portfolio

## Brand
- **Name:** Shreeram S. Kulkarni (Shreeram Kulkarni)
- **Tagline:** AI Automation Engineer — builds systems that replace busywork
- **Tone:** Technical, confident, self-taught authenticity, no corporate fluff
- **Audience:** Startup founders, agency partners, tech leads looking for automation leverage
- **Memorable thing:** "This person has built more automation than most teams — on his own, from scratch"

## Aesthetic
- **Mood:** Minimal, dark, technical — code editor meets design system
- **Energy:** Calm confidence, substance over flash
- **Material:** Glassmorphism-lite — subtle backdrop blur on nav, card surfaces with light borders, depth via noise texture overlay
- **Differentiators:**
  1. No stock imagery — every visual element is earned (code, icons, data)
  2. Motion as utility, not decoration — animations serve hierarchy and reveal, not gimmick
  3. Monospace elements woven into body type for technical flavor

## Color System
```css
--bg: #0a0a0b          /* Deep background — near black */
--bg-surface: #121214  /* Elevated surfaces, nav background */
--bg-card: #1a1a1e     /* Card surfaces */
--bg-card-hover: #222228
--border: #2a2a30      /* Subtle borders */
--text-primary: #f4f4f5 /* High-emphasis text */
--text-secondary: #a1a1aa /* Body text */
--text-muted: #6b6b7a   /* Low-emphasis text */
--accent: #22d3ee       /* Cyan — primary interactive color */
--accent-dim: #0891b2   /* Darker accent for depth */
--accent-glow: rgba(34, 211, 238, 0.15) /* Glow effect */
--green: #4ade80        /* Status indicators */
--amber: #fbbf24        /* Warning/highlight */
--gradient: linear-gradient(135deg, #22d3ee 0%, #a78bfa 60%, #f472b6 100%)
```

## Typography
- **Headings:** Inter (600–800 weight) — tight letter-spacing -0.04em, responsive clamp sizing
- **Body:** Inter 400, 1.6 line-height for readability
- **Code / tags / stats:** JetBrains Mono (monospace) for technical flavor
- **Gradient text:** On hero headline and accent spans

## Layout
- **Max-width:** 1100px content
- **Section padding:** 100px top/bottom (80px on mobile)
- **Grid:** Auto-fill minmax(320px, 1fr) for cards
- **Cards:** 12px border-radius, 28px padding, border, subtle shadow
- **Timeline:** Left-rail dot indicator with gradient accent

## Motion System
- **Typewriter:** Hero headline types in char-by-char, then cursor blinks
- **Fade-up:** Sections reveal on scroll with 30px upward translate, 0.6s ease-out
- **Stagger children:** Cards within grid reveal sequentially (0.1s delay per card)
- **Hover lift:** Cards translateY(-2px) on hover with 0.3s ease
- **Scale pulse:** Status dot pulses infinite 2s ease-in-out
- **Gradient drift:** Gradient text animates position subtly
- **Nav blur:** 0.3s transition on backdrop-blur
- **Glow:** Buttons glow on hover with radial shadow
- **Float:** Hero gradient orb moves subtly on page scroll
- **All animations use `prefers-reduced-motion: no-preference`** — accessibility, not assumption

## Responsive Breakpoints
- **Desktop:** 1100px max-width
- **Tablet:** 768px — stacks 2-column grids to 1, adjusts padding
- **Mobile:** Single column, smaller type (~2.2rem hero), full-width sections

## Anti-Slop Rules
- No decorative blobs, waves, or SVG ornaments
- No three-column icon grids
- No centered everything
- No purple gradients as primary design element
- No stock photography
- No fake statistics
