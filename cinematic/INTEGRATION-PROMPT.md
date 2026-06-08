# Cinematic Components — Designer Integration Prompt

These 30 modules are standalone HTML files (vanilla HTML + CSS + JS). Most of the scroll-driven ones load GSAP 3 + ScrollTrigger from a CDN; several others (e.g. `particle-button.html`, `dock-nav.html`, `flip-cards.html`, `gradient-stroke.html`) are pure CSS / vanilla JS with no dependencies. To add one to your own project, paste the prompt below into Claude Code / Cursor / any coding AI, then attach the module's `.html` file.

## Copy-paste prompt

```
I want to add a cinematic UI component to my project. The component is a single
self-contained HTML file (vanilla HTML + CSS + JS). Some modules also use GSAP 3
+ ScrollTrigger from a CDN; others are pure CSS / vanilla JS with no dependencies.
Source: the "Cinematic Site Modules" library by RoboLabs.

Here is the component file: [paste/attach the <module>.html, e.g. text-mask.html]

My project stack is: [e.g. Next.js App Router / Vite + React / plain HTML / Astro].

Please:
1. Extract the component's markup, CSS, and JS into the idiomatic form for my stack
   (e.g. a React component + useEffect for any JS init, or a scoped <section> for
   plain HTML).
2. First check whether the attached file actually uses GSAP (look for a gsap CDN
   <script> or gsap.* calls). Only if it does, load GSAP + ScrollTrigger the right
   way for my stack (CDN <script> for static sites; `npm i gsap` + dynamic import
   for bundled apps — register ScrollTrigger with gsap.registerPlugin(ScrollTrigger)).
   If the module is pure CSS / vanilla JS, do NOT add GSAP.
3. Scope the styles so they don't leak into the rest of my site (CSS module,
   styled component, or a unique wrapper class — not bare global selectors).
4. Map the component's hard-coded colors/fonts to my design tokens: [list your
   tokens, or say "use my existing CSS variables"].
5. Make it responsive and respect prefers-reduced-motion (disable/shorten the
   animation when the user opts out).
6. Tell me exactly where to mount it and show the import/usage snippet.

Keep the animation behavior identical to the original. Don't add dependencies
beyond what the component already uses (only GSAP if it's actually present).
Surgical changes only.
```

## The 30 modules

| # | File | Category | Effect |
|---|------|----------|--------|
| 01 | `text-mask.html` | Scroll-Driven | Headline fills with colour as you scroll |
| 02 | `sticky-stack.html` | Scroll-Driven | Product pins, features scroll past it |
| 03 | `zoom-parallax.html` | Scroll-Driven | Depth layers, foreground zooms past |
| 04 | `horizontal-scroll.html` | Scroll-Driven | Vertical scroll → horizontal gallery |
| 05 | `sticky-cards.html` | Scroll-Driven | Cards pin and stack on each other |
| 06 | `svg-draw.html` | Scroll-Driven | Lines draw themselves on scroll |
| 07 | `curtain-reveal.html` | Scroll-Driven | Hero splits open like curtains |
| 08 | `split-scroll.html` | Scroll-Driven | Two halves scroll opposite directions |
| 09 | `color-shift.html` | Scroll-Driven | Background changes per section |
| 10 | `cursor-reactive.html` | Cursor & Hover | Glow, 3D tilt, magnetic buttons, ripples |
| 11 | `accordion-slider.html` | Cursor & Hover | Strips expand on hover |
| 12 | `cursor-reveal.html` | Cursor & Hover | Before/after with wipe, spotlight, split |
| 13 | `image-trail.html` | Cursor & Hover | Cursor leaves fading images behind |
| 14 | `flip-cards.html` | Cursor & Hover | Cards rotate to reveal back |
| 15 | `magnetic-grid.html` | Cursor & Hover | Tiles push away from cursor |
| 16 | `spotlight-border.html` | Cursor & Hover | Borders illuminate under cursor |
| 17 | `drag-pan.html` | Cursor & Hover | Infinite draggable canvas |
| 18 | `view-transitions.html` | Click & Tap | Elements shape-shift between states |
| 19 | `particle-button.html` | Click & Tap | CTAs burst on click |
| 20 | `odometer.html` | Click & Tap | Digit wheels roll to target |
| 21 | `coverflow.html` | Click & Tap | Center focused, edges angled |
| 22 | `dynamic-island.html` | Click & Tap | Pill morphs for notifications |
| 23 | `dock-nav.html` | Click & Tap | Icons magnify on hover |
| 24 | `text-scramble.html` | Ambient & Auto | Matrix-style character cycling |
| 25 | `kinetic-marquee.html` | Ambient & Auto | Infinite text bands, scroll-reactive |
| 26 | `mesh-gradient.html` | Ambient & Auto | Animated colour blobs |
| 27 | `circular-text.html` | Ambient & Auto | Text on spinning circle |
| 28 | `glitch-effect.html` | Ambient & Auto | RGB channel split |
| 29 | `typewriter.html` | Ambient & Auto | Text types itself |
| 30 | `gradient-stroke.html` | Ambient & Auto | Animated gradient on outlined text |

## Attribution & License

Components created by Jay from RoboLabs — <https://robonuggets.com>.

These demos are MIT licensed by their author. The full upstream copyright and MIT
license text is included alongside this folder in
[`LICENSE-cinematic-components`](./LICENSE-cinematic-components) (`Copyright (c) 2026
Jay from RoboLabs`), as MIT requires the notice to travel with the code.
