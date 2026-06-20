<div align="center">
  <br/>
  <img src="./public/images/nav-logo.svg/" alt="SPYLT Logo" width="80"/>
  <h1 align="center">SPYLT — Freaking Delicious</h1>
  <p align="center">
    <strong>Brand landing page built with React · GSAP · Tailwind CSS</strong>
  </p>
  <p align="center">
    <a href="https://spylt-clone.onrender.com/" target="_blank"><strong>🌐 Live Demo</strong></a>
  </p>
  <br/>
</div>

---

## 📋 Overview

SPYLT is a high-fidelity brand landing page for a fictional protein + caffeine milk drink. Every section is crafted with **scroll-driven animations** using the full GSAP ecosystem — ScrollSmoother, ScrollTrigger, SplitText, clip-path reveals, pinned horizontal carousels, and staggered parallax effects.

Built to demonstrate **production-quality front-end engineering** with a focus on motion design, responsive architecture, and visual polish.

---

## ✨ Key Features

| Feature | Implementation |
|---|---|
| **Smooth Scrolling** | GSAP ScrollSmoother with `smooth: 3` for fluid, butter-like scroll |
| **Scroll-Driven Animations** | Every section uses ScrollTrigger with scrub, pin, and stagger |
| **Character Splits** | SplitText breaks headlines into individual chars for cascading reveals |
| **Word-by-Word Reveals** | Paragraphs animate word-by-word with rotation for elegant text entrances |
| **Horizontal Carousel** | Pinned horizontal scroll for the 6-flavor product showcase |
| **Clip-Path Reveals** | Polygon/circle clip-paths animate from center/edge to reveal content |
| **Video Pin Expansion** | Pinned video grows from a tiny 6% circle to full-screen on scroll |
| **Parallax Depth** | Multi-speed horizontal movement on testimonial titles |
| **Staggered Card Deck** | Testimonial cards slide up in sequence with alternating rotations |
| **Fully Responsive** | Desktop, tablet (≤1024px), and mobile (≤768px) breakpoints with adapted layouts |

---

## 🎬 Animation Breakdown

### ScrollSmoother — App-wide
The entire page is wrapped in GSAP's ScrollSmoother, overriding the native scroll wheel with a smooth, accelerated feel. The navbar lives outside the wrapper to stay fixed.

### Hero Section — Entry + Exit
- Page-load entry: content fades up and clip-path opens from center
- Character stagger: "Freaking Delicious" splits into individual chars, each animating from below
- Scroll exit: the entire hero container rotates 7° and scales down as you scroll away

### Message Section — Slow Word Color Reveal
- Words transition from transparent to visible with a 1-second stagger gap per word
- Creates an elegant, slow-motion reading experience

### Flavor Section — Pinned Horizontal Scroll
- The flavor title splits into characters cascading from below
- The flavor slider **pins in place** while its cards scroll horizontally
- 6 drink cards tilt in alternating rotations (-8° / 8°)

### Nutrition Section — Text + Data Reveal
- Title characters cascade in from below
- Paragraph words animate from below with rotation
- Badge clip-path opens from right to left

### Benefit Section — Staggered Clip-Path Titles
- Four benefit titles reveal sequentially, each opening from a centered vertical line to full width
- Ends with the signature **video pin** effect

### Video Pin Section — Circle Expansion
- Desktop: video starts as a tiny `circle(6%)` dot and expands to `circle(100%)`
- Overlaid with a continuously spinning circular text SVG
- Pinned across a large scroll distance for dramatic reveal

### Testimonial Section — Parallax + Card Stagger
- Three title lines move horizontally at different speeds (parallax)
- 7 video cards pin in place and stagger in from below with different rotations
- Hover to play testimonial videos

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **React 19** | Component architecture |
| **Vite 8** | Build tool & HMR |
| **GSAP 3.15** | All animations — ScrollTrigger, ScrollSmoother, SplitText |
| **@gsap/react** | `useGSAP()` hook for React lifecycle-safe animations |
| **Tailwind CSS v4** | Utility-first styling with custom design tokens |
| **react-responsive** | `useMediaQuery()` for responsive breakpoints |

---

## 📁 Project Structure

```
src/
├── components/           # Reusable UI pieces
│   ├── ClipPathTitle.jsx   # Animated title with clip-path reveal
│   ├── FlavorTitle.jsx     # SplitText character animation title
│   ├── FlavorSlider.jsx    # Horizontal pinned carousel
│   ├── Navbar.jsx          # Fixed top-left branding
│   └── VideoPinSection.jsx # Circle-expanding video pin
├── constants/            # Data definitions
│   └── index.js            # Flavors, nutrients, testimonials
├── sections/             # Full-page sections
│   ├── HeroSection.jsx
│   ├── MessageSection.jsx
│   ├── FlavorSection.jsx
│   ├── NutritionSection.jsx
│   ├── BenefitSection.jsx
│   ├── TestimonialSection.jsx
│   └── FooterSection.jsx
├── App.jsx               # Root — ScrollSmoother wrapper
├── index.css             # Tailwind v4 + custom styles
└── main.jsx              # Entry point
```

---

## 🎯 What This Demonstrates

- **Advanced GSAP:** ScrollSmoother, ScrollTrigger (pin, scrub, stagger), SplitText (chars/words), clip-path animations, timeline sequencing, responsive scroll disabling
- **React Best Practices:** Component composition, hooks, responsive state management, lifecycle-safe animations with `useGSAP()`
- **Responsive Design:** Tailwind CSS with custom theme tokens, three-tier breakpoint system, adaptive layouts that swap videos for images on mobile
- **Visual Craft:** Cohesive color palette, custom typography (Antonio + ProximaNova), polished micro-interactions, sticky/fixed positioning

---

<div align="center">
  <br/>
  <p>
    Built with <strong>React</strong>, animated with <strong>GSAP</strong>, styled with <strong>Tailwind CSS</strong>
  </p>
  <p>
    <a href="https://spylt-clone.onrender.com/" target="_blank"><strong>🌐 Live Demo →</strong></a>
  </p>
  <br/>
</div>
