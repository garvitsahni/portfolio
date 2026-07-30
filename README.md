# Garvit Sahni — Portfolio

Single-page dark-theme portfolio built with GSAP, Lenis, and a frame-based scroll canvas. Features glass morphism, custom cursor, and smooth scroll-driven video playback.

## Tech

- **GSAP 3.12.5** + **ScrollTrigger** — scroll-driven reveals, hero intro, practice panel pinning
- **Lenis 1.0.42** — smooth scrolling with easing
- **Canvas frame animation** — 300 PNG frames synced to scroll position
- **Google Fonts** — Playfair Display, JetBrains Mono, Inter
- **Formspree** — contact form endpoint

## File structure

```
G portofilio/
├── scroll-animation/
│   ├── index.html          ← main portfolio (single file)
│   └── Resume_Garvit.pdf
├── extracted_frames_30fps/  ← 300 scroll video frames
├── archive/                 ← light-theme version (deprecated)
└── README.md
```

## Local dev

No build step — open the file directly:

```
start scroll-animation/index.html
```

Works from any static server or local file:// (frames load relative to `../extracted_frames_30fps/`).

## Resilience

The animation layer is guarded against CDN failure — if gsap.min.js, ScrollTrigger.min.js, or lenis.min.js fail to load, all content remains fully visible via CSS defaults. No content is ever hidden-until-animated.

## Links

- [GitHub](https://github.com/garvitsahni)
- [LinkedIn](https://linkedin.com/in/garvit-sahni-0a8826325)
