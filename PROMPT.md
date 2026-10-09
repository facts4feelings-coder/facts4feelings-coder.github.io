# TechMint: "Corporate Live Studio" (AI website prompt)

Copy everything below into Lovable / Bolt / v0 / Cursor / Claude.

---

Build a professional, corporate, trustworthy marketing website for **TechMint (techmint.org)**, a web studio with two services:
1. **New Website Development**: professional websites built from scratch.
2. **Website Redesign**: turning old, slow, non-mobile websites into modern, fast ones while keeping content and Google rankings.

## Audience & tone
Normal business owners (clinics, bakeries, shops, builders), not developers. The copy must be simple and benefit-focused ("loads fast", "perfect on phones", "shows up on Google"). The design should still feel premium and techy, using coding fonts, small code accents, sounds, and animation as *style*, never as jargon the visitor has to understand.

## Visual style
- **Look:** clean corporate, mostly white with confident blue (Stripe / Vercel / modern SaaS level polish)
- **Fonts:** Sora (headings), Inter (body), JetBrains Mono (labels, code panel, small accents such as `new_website()` tags)
- **Light:** bg #FFFFFF, soft #F5F8FF, text navy #0B1B3F, muted #5A6B8C, border #E2E9F5, blue #2563EB (hover #1D4ED8), light blue #E8F0FF
- **Dark:** bg #060D1F, surface #0D1833, text #EAF0FF, blue #4F8BFF
- Subtle grid pattern in the hero, 10–20px radii, soft shadows, fade-up scroll reveals, hover lifts
- Real photography (team, client businesses), not illustrations

## THE HERO: "TechMint Studio" live panel (the main wow factor)
Headline: "We build **new websites** and make old ones **new again.**", two CTAs, and a small "turn on sound 🔊" link.
Below it, a large app-like window (macOS dots, title "TechMint Studio — project-name", a LIVE badge) with two tabs: **✦ Build new website** | **↻ Old → New**. The panel auto-plays and loops between both modes. Layout: left sidebar of steps (spinner → green check), a middle dark code editor, and a right live browser preview.

**Build mode:** the code editor types simple, readable lines with comments (`// 1. Add the header` → `<Header logo="Saffron Bakery" />`). After each line, that element appears in the live preview with a pop and a blue highlight: header → headline typing → real photo → button → 3 feature cards. Then `responsive()` shrinks the preview to a phone and back, and `deploy()` shows a "Your website is live! ✓" overlay. A progress bar fills as it goes.

**Old → New mode:** the preview shows an ugly 2010-style clinic website. The editor runs `audit("citycareclinic.com")` and red flags pop onto the preview (✗ SLOW 6.4s, ✗ NOT MOBILE FRIENDLY, ✗ OUTDATED DESIGN), turning sidebar items red. Then `redesign({ keepContent: true, keepSEO: true })` runs and a glowing blue scan line sweeps top-to-bottom, revealing the modern redesigned site underneath while a speed meter climbs from 34 to 98. Green ✓ lines follow, then a "Old website → brand new!" overlay.

## Other sections
1. Trust numbers with count-up (120 websites, 60+ businesses, 3× faster, 24h reply)
2. Services: two big cards with photo headers (New Website / Redesign with a before|after split thumbnail), checklists, CTAs
3. Why TechMint: team photo with a rating badge + 3 features (hand-coded, fast & mobile-first, clear pricing)
4. How it works: 4 steps on a connecting line that draws in on scroll
5. Case study: City Care Clinic with a draggable before/after slider + result cards (6.4s → 0.9s, +180% bookings)
6. Testimonials: 3 cards
7. Contact: navy-to-blue gradient block + white form (New/Redesign choice; Redesign reveals a "current website" field) and a success state
8. Footer with 4 columns

## Sound design (Web Audio API, MUTED by default, speaker toggle in the navbar, remembered)
Soft keyboard clicks while the code types, a gentle "pop" when an element appears, a low "error" tone for red flags, a whoosh for the scan sweep and phone resize, a 4-note success chime on launch/form submit, and very light hover ticks.

## Technical
Next.js + TypeScript + Tailwind + Framer Motion. Dark/light toggle (system default, localStorage, no flash). Responsive 360–1920px (panel stacks on mobile; the sidebar hides). Accessible (WCAG AA, focus states, prefers-reduced-motion). Optimized images, SEO meta. Clean, componentized code with content in data files.
