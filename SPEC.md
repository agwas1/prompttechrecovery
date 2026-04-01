# PromtTech Recovery - Crypto Recovery Services Website

## Concept & Vision

A trustworthy, authoritative website for a crypto recovery startup that helps victims of scams, hacks, and lost access recover their digital assets. The site should convey technical expertise, security consciousness, and genuine empathy for clients who have lost funds. The feeling is "elite cyber security firm meets financial recovery specialists."

## Design Language

### Aesthetic Direction
Dark, sophisticated tech aesthetic inspired by cybersecurity dashboards and fintech platforms. Think Bloomberg Terminal meets Mr. Robot - data-dense yet accessible, with strategic use of glowing accents suggesting blockchain/network connectivity.

### Color Palette
- **Primary Background**: `#0a0e17` (deep space black)
- **Secondary Background**: `#111827` (card surfaces)
- **Tertiary**: `#1e293b` (elevated elements)
- **Primary Accent**: `#10b981` (emerald green - trust, money, success)
- **Secondary Accent**: `#06b6d4` (cyan - blockchain, tech)
- **Warning**: `#f59e0b` (amber - urgency, attention)
- **Text Primary**: `#f1f5f9`
- **Text Secondary**: `#94a3b8`
- **Text Muted**: `#64748b`

### Typography
- **Headings**: "Space Grotesk" (geometric, tech-forward) - bold weights
- **Body**: "Inter" (clean, highly legible) - regular/medium weights
- **Monospace accents**: "JetBrains Mono" (for crypto addresses, stats)

### Spatial System
- Base unit: 8px
- Section padding: 80px vertical on desktop, 48px on mobile
- Container max-width: 1200px
- Card border-radius: 12px
- Button border-radius: 8px

### Motion Philosophy
- Entrance animations: fade-up with stagger (100ms delays)
- Hover states: subtle scale (1.02) with glow effect
- Number counters: animated count-up for statistics
- Floating particles: subtle blockchain/network node visualization
- Scroll-triggered reveals using Intersection Observer

### Visual Assets
- Lucide icons (consistent stroke weight)
- Custom SVG illustrations for services
- Animated gradient mesh background
- Subtle grid pattern overlay

## Layout & Structure

### Navigation
Fixed top nav with blur backdrop, logo left, links center, CTA right. Transforms to hamburger menu on mobile.

### Sections (in order)
1. **Hero** - Full viewport, animated headline, subtext about mission, dual CTAs (Start Recovery / Learn More), floating crypto icons animation
2. **Trust Bar** - Scrolling logos of crypto networks/protocols supported
3. **Services** - 3-4 service cards in grid: Stolen Funds Recovery, Lost Wallet Access, Scam Victim Support, Smart Contract Dispute
4. **How It Works** - 4-step numbered process with connecting lines
5. **Statistics** - Large animated counters: recovery rate, funds recovered, cases handled, success years
6. **Why Choose Us** - Feature grid with icons
7. **Testimonials** - Carousel of client success stories (anonymous/starred names)
8. **FAQ** - Accordion style common questions
9. **CTA Section** - Full-width gradient, final push to contact
10. **Footer** - Links, contact info, legal disclaimers, social icons

## Features & Interactions

### Hero Section
- Typewriter effect on headline cycling through recovery scenarios
- Floating animated crypto symbols (BTC, ETH, USDT icons) drifting
- Primary CTA: "Start Recovery Process" → opens modal/redirect
- Secondary CTA: "View Our Process" → smooth scroll to how-it-works

### Service Cards
- Hover: card lifts, border glows with accent color
- Icon animates (subtle pulse or rotation)
- Each links to expanded service detail (or accordion)

### Statistics Counter
- Numbers animate from 0 to final value on scroll into view
- Duration: 2 seconds, easing
- Suffixes: %, $, + symbols

### Testimonials
- Auto-rotating carousel (5s interval)
- Manual navigation dots
- Pause on hover

### FAQ Accordion
- Click to expand/collapse
- Smooth height animation
- Plus/minus icon rotation

### Contact/CTA Modal (optional)
- Form: name, email, crypto type, brief description, preferred contact time
- Validation with inline error messages
- Success state with confirmation message

## Component Inventory

### Button
- Primary: emerald bg, white text, hover glow
- Secondary: transparent, border, hover fill
- States: default, hover (glow + slight lift), active (pressed), disabled (muted)

### Card
- Dark bg with subtle border
- Hover: border color shifts to accent, subtle shadow
- Contains: icon, title, description, optional link

### Navigation Link
- Default: muted text
- Hover: primary text, underline animation
- Active: accent color

### Stat Block
- Large number (animated)
- Label below
- Optional icon

### Testimonial Card
- Avatar placeholder (initials)
- Star rating
- Quote text
- Name (partially obscured for privacy)

### FAQ Item
- Collapsible header with question
- Hidden body with answer
- Expand/collapse icon

## Technical Approach

- **Framework**: Single HTML file with embedded CSS and vanilla JavaScript
- **CSS**: Custom properties for theming, CSS Grid and Flexbox for layout
- **JavaScript**: Intersection Observer for scroll animations, custom carousel, accordion logic
- **Fonts**: Google Fonts (Space Grotesk, Inter, JetBrains Mono)
- **Icons**: Lucide icons via CDN
- **Animations**: CSS animations + keyframes, JS for counters and scroll triggers
- **Responsive**: Mobile-first, breakpoints at 640px, 768px, 1024px, 1280px
