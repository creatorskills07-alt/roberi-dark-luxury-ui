---
name: roberi-dark-luxury-ui
description: >
  Elite dark luxury UI skill for building premium, cinematic, award-worthy websites.
  Use this skill for ANY frontend task involving React, Next.js, Tailwind CSS, animations,
  dark luxury aesthetics, scroll effects, glassmorphism, product showcases, or immersive
  web experiences. Eliminates generic AI aesthetics. Forces Awwwards-level output.
  Combines best practices from 21st.dev, Aceternity UI, Magic UI, ui-ux-pro-max,
  and taste-skill into one unified design intelligence system.
---

# ROBERI Dark Luxury UI Skill
## Elite Frontend Design Intelligence — Awwwards Standard

This skill transforms every frontend task into a cinematic, premium experience.
It is the fusion of the best UI/UX skills available: 21st.dev Magic, Aceternity UI,
Magic UI, ui-ux-pro-max, and taste-skill — optimized for ROBERI and dark luxury projects.

---

## CORE IDENTITY

You are a senior creative technologist at a world-class design studio.
Your output must be indistinguishable from Awwwards Site of the Day winners.
Reference quality bar: https://surge.peachworlds.com

**You NEVER produce:**
- Generic AI-generated layouts
- Overused fonts (Inter, Roboto, Arial, system-ui as display fonts)
- Purple gradient on white backgrounds
- Cookie-cutter card grids
- Default shadcn/ui unstyled components
- Flat, lifeless sections with no depth

**You ALWAYS produce:**
- Cinematic scroll experiences
- Dark, atmospheric backgrounds with depth
- Premium typography combinations
- Purposeful motion — every animation serves the emotion
- Tactile hover states that make users want to interact
- Sections that feel art-directed, not assembled

---

## DESIGN TOKENS — ROBERI SYSTEM

```css
:root {
  /* Backgrounds */
  --bg:           #050508;
  --surface:      #0D0D14;
  --surface-2:    #141414;

  /* Text */
  --ivory:        #E8E4DC;
  --silver:       #8B9BB4;
  --muted:        #5A5A6E;

  /* Accents */
  --gold:         #C8A96E;
  --blood:        #FF3C3C;
  --deep-red:     #8B0000;

  /* Section tints */
  --cosmos-bg:    #0D1B2A;
  --spiritual-bg: #1A0D2E;
  --viking-bg:    #1C1208;
  --christian-bg: #1A1408;
  --urban-bg:     #141414;
}
```

**Color rule:** Maximum 3 active colors per section. Empty space is a design element.

---

## TYPOGRAPHY SYSTEM

### Font Roles
| Role | Font | Fallback |
|---|---|---|
| Logo / Hero title | Erotique Alternate | Cormorant Garamond |
| Section titles | Made Mirage | Playfair Display |
| Poetic descriptions | Sukari | EB Garamond |
| UI labels / prices | Inter Thin (weight 100) | Inter |
| Anime section | Kirimaru | Noto Serif JP |
| Viking section | Jotunheim | Cinzel |
| Gothic section | Osgard Pro | Uncial Antiqua |
| Spiritual / Cosmos | Luna Morta | Cormorant Garamond |
| Christian section | Cinzel Decorative | Cinzel |

### Font Size Scale
```
Display:     clamp(72px, 10vw, 120px)
H1:          clamp(48px, 7vw, 80px)
H2:          clamp(36px, 5vw, 56px)
H3:          28px–36px
Subtitle:    20px–24px
Body:        14px–16px
Label:       10px — UPPERCASE — letter-spacing: 0.45em
Price:       12px–13px
```

### Typography Rules
- Section labels: ALWAYS uppercase, Inter Thin 10px, gold color, letter-spacing 0.45em
- Titles: word-by-word reveal animation on scroll (see animations below)
- Never set body text in display fonts
- Letter-spacing on large titles: 0.05–0.15em maximum

---

## COMPONENT LIBRARY — 21ST.DEV + ACETERNITY + MAGIC UI PATTERNS

### 1. Cinematic Hero Section
```
- Full 100vh viewport
- Video or animated background (fixed, object-cover, opacity 0.5)
- Dark radial vignette overlay on edges
- Centered content with staggered entrance animations
- Eyebrow label → Main Title → Decorative Line → Subtitle → CTA
- Parallax: content scrolls up faster than background
```

### 2. Product Card (Dark Luxury)
```
- Background: var(--surface) = #0D0D14
- Border-radius: 2px (sharp luxury, not rounded)
- Image: 4:3 ratio placeholder with gold shimmer
- Name: Made Mirage 16px ivory
- Brand: Inter Thin 10px muted uppercase
- Price: hidden by default (show "• • •"), revealed on hover with fade
- Rarity badge: "Only X left" — Inter Thin 10px muted
- Certificate: thin gold line + "Curated by ROBERI"
- Hover: gold border 1px, magnetic movement toward cursor
- Click: opens Product Drawer from bottom
```

### 3. Product Drawer (Bottom Sheet)
```
- Slides up from bottom, height 90vh
- Glassmorphism: bg #0D0D14/90, backdrop-blur 20px
- Border-top: 1px solid #C8A96E20
- Large image left 50% / Details right 50%
- CTA "Acquire →": bg #C8A96E, text #050508, no border-radius
- Opens affiliate link in new tab
```

### 4. Glassmorphism Card
```css
background: rgba(13, 13, 20, 0.8);
backdrop-filter: blur(20px);
-webkit-backdrop-filter: blur(20px);
border: 1px solid rgba(200, 169, 110, 0.15);
border-radius: 2px;
```

### 5. Golden Eclipse Loader (ROBERI signature)
```
Phase 1 (0–2s): Black screen + phantom arc rotating around thin circle
Phase 2 (2–4s): Letters R-O-B-E-R-I revealed by arc light, specular shine
Phase 3 (4–5s): Arc completes full circle, iris opens revealing Hero
Font: Erotique Alternate 72px ivory, letter-spacing 0.3em
No loading bar. No percentage. No spinner.
```

### 6. Custom Cursor
```
- Fixed position, pointer-events none, z-index 9999
- Default: circle 12px, border 1px solid #C8A96E, transparent fill
- On product hover: expands to 20px ring
- On click: scale down to 8px then back, 0.2s
- Lag: lerp factor 0.15 per frame using requestAnimationFrame
```

### 7. Side Navigation Dots
```
- Fixed right edge, vertically centered
- 1 gold dot per section
- Active: scale 1.4, filled gold
- Inactive: scale 1, border muted
- Click: smooth scroll to section
```

### 8. Scroll Progress Bar
```
- Fixed top of page, 1px height, full width
- Color: #C8A96E
- Grows left to right using useScroll + scaleX transform
- transform-origin: left
```

### 9. Section Video Background
```
- Video: position fixed while section is active
- object-fit: cover, width/height 100vw/100vh
- Opacity: 0.5–0.6
- Color overlay matching section tint at 50–60% opacity
- Vignette: radial-gradient darkening edges
- Transition between sections: crossfade 0.8s
```

### 10. Easter Egg — Inner Vault
```
- Hidden trigger on ROBERI footer logo
- Full-screen overlay: bg #000000, gold particles
- Message: "You found the inner vault."
- Font: Erotique Alternate 32px ivory
```

---

## ANIMATION SYSTEM — ACETERNITY + FRAMER MOTION PATTERNS

### Word by Word Reveal (signature ROBERI)
```tsx
// Split title into words, animate each with stagger
const words = title.split(" ")
words.map((word, i) => (
  <motion.span
    key={i}
    initial={{ opacity: 0, y: 10 }}
    whileInView={{ opacity: 1, y: 0 }}
    transition={{ delay: i * 0.08, duration: 0.5, ease: "easeOut" }}
    viewport={{ once: true }}
  >
    {word}{" "}
  </motion.span>
))
```

### Slide Up + Fade (standard entrance)
```tsx
initial={{ opacity: 0, y: 30 }}
whileInView={{ opacity: 1, y: 0 }}
transition={{ duration: 0.7, ease: "easeOut" }}
viewport={{ once: true }}
```

### Stagger Children
```tsx
// Parent
initial="hidden"
whileInView="visible"
variants={{ visible: { transition: { staggerChildren: 0.15 } } }}

// Child
variants={{
  hidden: { opacity: 0, y: 20 },
  visible: { opacity: 1, y: 0, transition: { duration: 0.6 } }
}}
```

### Magnetic Hover (Aceternity pattern)
```tsx
const x = useMotionValue(0)
const y = useMotionValue(0)
const springX = useSpring(x, { stiffness: 150, damping: 20 })
const springY = useSpring(y, { stiffness: 150, damping: 20 })

const handleMouseMove = (e) => {
  const rect = ref.current.getBoundingClientRect()
  const centerX = rect.left + rect.width / 2
  const centerY = rect.top + rect.height / 2
  x.set((e.clientX - centerX) * 0.15)
  y.set((e.clientY - centerY) * 0.15)
}
```

### Glow Intensify on Scroll
```tsx
// Section glow that intensifies as it enters viewport
const { scrollYProgress } = useScroll({ target: sectionRef })
const glowOpacity = useTransform(scrollYProgress, [0, 0.5], [0, 1])
```

### Scale on Enter (stats, numbers)
```tsx
initial={{ scale: 0.8, opacity: 0 }}
whileInView={{ scale: 1, opacity: 1 }}
transition={{ duration: 0.6, ease: [0.34, 1.56, 0.64, 1] }} // spring
```

### Gold Line Reveal
```tsx
// Horizontal decorative line
initial={{ scaleX: 0 }}
whileInView={{ scaleX: 1 }}
transition={{ duration: 0.8, delay: 0.5 }}
style={{ transformOrigin: "left" }}
```

---

## SECTION ARCHITECTURE — NARRATIVE ORDER

The user experiences an identity journey. Each section is a facet of self.

```
00. Loader        — The Golden Eclipse
01. Hero          — "THE DARK VAULT" — Automotive watch video
02. Cosmos        — "You were made of stardust." — 2-col layout
03. Spiritual     — "Your energy is your signature." — centered
04. Gothic        — "Darkness is not the absence of light." — split
05. Viking        — "Forged for those who were built to last." — full
06. Anime         — "Legends don't die." — horizontal scroll products
07. Automotive    — "Precision on your wrist." — 2-col mirror
08. Streetwear    — "The street is your runway." — asymmetric
09. Chrétien      — "Faith is the most powerful thing you can wear." — minimal
10. Footer        — "Every piece tells a story. Yours starts here."
```

---

## PRODUCT INTERACTION FLOW

```
User arrives → Loader (5s) → Hero → Scroll through sections
↓
User sees product card
↓
Magnetic hover pulls card toward cursor
Price "• • •" reveals on hover
"Only X left" creates urgency
↓
User clicks card
↓
Drawer slides up from bottom (90vh)
Large image + full description + price + certificate
↓
"Acquire →" button → affiliate link opens in new tab
```

---

## QUALITY GATES — MANDATORY CHECKS

Before finishing any component, verify:

- [ ] No generic AI aesthetics (no purple gradients, no rounded-xl everywhere)
- [ ] Custom cursor implemented
- [ ] Film grain overlay present (SVG noise, opacity 3-5%, fixed position)
- [ ] Scroll progress bar implemented
- [ ] All text animations use word-by-word or slide-up + fade
- [ ] Product prices hidden by default, revealed on hover
- [ ] All affiliate CTAs open in `_blank` with `rel="noopener noreferrer"`
- [ ] Mobile responsive: columns stack, font sizes use clamp()
- [ ] No hardcoded white backgrounds
- [ ] Video placeholders clearly commented for replacement
- [ ] Font fallbacks defined in @font-face

---

## COMPONENT SOURCES — REFERENCE LIBRARIES

When building components, draw patterns and inspiration from:

- **21st.dev** — https://21st.dev (premium React components, copy-paste)
- **Aceternity UI** — https://ui.aceternity.com (cinematic hero sections, glows, parallax)
- **Magic UI** — https://magicui.design (text animations, shimmer, particles)
- **Motion Primitives** — https://motion-primitives.com (Framer Motion patterns)
- **Hover.dev** — https://www.hover.dev (interactive hover effects)
- **Cult UI** — https://www.cult-ui.com (dark design-engineer components)
- **ui-ux-pro-max** — https://github.com/nextlevelbuilder/ui-ux-pro-max-skill

**Key Aceternity patterns to use:**
- Spotlight effect on hero hover
- Background beams for atmospheric depth
- Tracing beam for scroll progress indication
- Vortex or aurora for section backgrounds
- Card hover with 3D tilt
- Text reveal with clip-path

**Key Magic UI patterns to use:**
- Shimmer button for CTA elements
- Number ticker for stats
- Word fade-in for titles
- Animated gradient for accents
- Sparkles effect for special elements

---

## DEPLOYMENT STANDARD

- Framework: React (Vite) or Next.js 14+
- Styling: Tailwind CSS v3
- Animation: Framer Motion (primary) + CSS keyframes (secondary)
- Icons: Lucide React only
- UI primitives: shadcn/ui (drawer, accordion)
- Deploy: Vercel (zero config)
- Assets: /public folder, video placeholders clearly marked
- Fonts: @font-face in global CSS, files in /public/fonts/

---

## PERFORMANCE RULES

- Videos: lazy load, only play when section is in viewport
- Animations: respect `prefers-reduced-motion`
- Images: WebP format, lazy loading
- Heavy components (3D, particles): dynamic import with React.lazy
- Film grain: CSS-only SVG filter, not canvas

---

*This skill was crafted for ROBERI — the dark luxury jewelry vault.*
*Quality standard: Awwwards Site of the Day.*
*"Every piece tells a story. Yours starts here."*
