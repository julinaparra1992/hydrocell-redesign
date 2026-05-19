---
version: 1.0
name: hydrocell-design-system
description: Hydrocell is a Colombian engine decarbonization brand using green hydrogen (HHO) technology. Premium-but-accessible automotive tech aesthetic, balancing scientific authority with environmental warmth. Cyan-teal primary anchored in deep ink with optional eco-green accents. Sans-serif system with confident headline weight and grounded body. Generous spacing, soft rounded corners, photography-heavy hero sections featuring real engines, technicians, and clean workshop environments.
---

# Hydrocell Design System

## 🎯 Brand Identity

- **Company:** HYDROCELL S.A.S — fundada en Medellín, Colombia (2013)
- **Sector:** Automotriz · descarbonización de motores con hidrógeno verde
- **Tagline:** "Mejoramos tu motor, el planeta y tu bolsillo te lo agradecen"
- **Audience:** Conductores particulares, taxistas, flotas empresariales colombianas
- **Tone:** Profesional, cálido, científico-accesible, NO corporativo aburrido, NO startup techy

## 🎨 Color Palette

```yaml
colors:
  # PRIMARY — cyan-teal (brand signature)
  primary: "#00b9b5"          # Bright teal — main brand color
  primary-dark: "#3bb4c3"     # Darker teal for hover states
  primary-deep: "#0a8a86"     # Deep teal for borders/accents
  primary-soft: "#cdefee"     # Soft tint for backgrounds
  primary-bg: "#e6f7f6"       # Lightest tint for hero washes

  # SECONDARY — eco green (sustainability accent)
  secondary: "#4EBD8D"        # Emerald — for eco messaging
  secondary-deep: "#3a9970"   # Darker green for CTAs
  secondary-soft: "#edf9f3"   # Soft tint

  # INK — text and structure
  ink-950: "#0a1620"          # Almost black, for dark sections
  ink-900: "#0e2f3e"          # Body text dark / nav
  ink-700: "#1a4a5e"          # Secondary text
  ink-500: "#5a7785"          # Muted text
  ink-300: "#94a3b8"          # Disabled / placeholder
  ink-100: "#e8eef2"          # Subtle borders
  ink-50:  "#f6f9fb"          # Section alt backgrounds

  # WHATSAPP — conversion accent (because all CTAs go to WhatsApp)
  whatsapp:  "#25d366"        # Official WhatsApp green
  whatsapp-dark: "#1da851"

  # SEMANTIC
  canvas: "#ffffff"
  canvas-cream: "#faf6f0"     # Warm alternative for eco variants
  success: "#4EBD8D"
  hairline: "#e0eaef"
```

## 🅰️ Typography

**Primary family:** Inter (universal modern sans, excellent multilingual)
**Display family:** Inter or Barlow Condensed (for aggressive variants)
**Mono:** JetBrains Mono (when used for technical labels)

```yaml
typography:
  display-xxl:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "72px"
    fontWeight: 800
    lineHeight: 1.05
    letterSpacing: "-0.02em"
  display-xl:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "56px"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "-0.015em"
  display-lg:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "40px"
    fontWeight: 700
    lineHeight: 1.15
  heading-lg:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "30px"
    fontWeight: 700
    lineHeight: 1.2
  heading-md:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "24px"
    fontWeight: 600
    lineHeight: 1.25
  body-lg:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.6
  body-md:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.6
  body-sm:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.5
  label-tiny:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "12px"
    fontWeight: 600
    letterSpacing: "0.15em"
    textTransform: "uppercase"
  numerals-display:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "72px"
    fontWeight: 800
    lineHeight: 1
    fontFeature: "tnum"  # tabular figures for stats
```

## 📐 Spacing System

```yaml
spacing:
  0:   "0"
  1:   "4px"
  2:   "8px"
  3:   "12px"
  4:   "16px"
  6:   "24px"
  8:   "32px"
  12:  "48px"
  16:  "64px"
  20:  "80px"
  24:  "96px"
  32:  "128px"

section-padding-mobile:  "64px 24px"
section-padding-desktop: "96px 24px"
container-max-width:     "1280px"   # max-w-7xl
content-max-width:       "896px"    # max-w-4xl for long-form
```

## 🔘 Shape System

```yaml
borderRadius:
  none:  "0"
  sm:    "6px"        # Small UI elements
  md:    "12px"       # Cards, inputs
  lg:    "16px"       # Service cards
  xl:    "24px"       # Hero cards, big containers
  2xl:   "32px"       # Soft variants (eco style)
  pill:  "9999px"     # Buttons, pills, chips
  badge: "9999px"

borderWidth:
  default: "1px"
  emphasis: "2px"     # On accent borders
  hairline: "1px"     # Internal dividers
```

## 🌈 Shadow System

```yaml
shadows:
  none: "none"
  sm:   "0 1px 2px rgba(14, 47, 62, 0.06)"
  md:   "0 4px 12px rgba(14, 47, 62, 0.08)"
  lg:   "0 12px 32px rgba(14, 47, 62, 0.12)"
  xl:   "0 24px 48px rgba(14, 47, 62, 0.15)"
  glow-cyan: "0 8px 24px rgba(0, 185, 181, 0.35)"
  glow-green: "0 8px 24px rgba(78, 189, 141, 0.35)"
  glow-whatsapp: "0 4px 16px rgba(37, 211, 102, 0.35)"
```

## 🧱 Component Standards

### Buttons

```yaml
button-primary:
  background: "primary (#00b9b5)"
  text: "white"
  hover: "primary-dark (#3bb4c3)"
  borderRadius: "pill"
  padding: "16px 32px"
  fontWeight: 600
  shadow: "glow-cyan"
  transition: "transform .15s, shadow .15s"

button-whatsapp:
  background: "linear-gradient(135deg, #25d366, #1da851)"
  text: "white"
  shadow: "glow-whatsapp"
  hover: "translateY(-2px)"
  use: "Always for CTAs to WhatsApp"

button-secondary:
  background: "transparent"
  border: "2px solid primary"
  text: "primary"
  hover-bg: "primary-soft"

button-ghost:
  background: "transparent"
  text: "ink-700"
  hover-text: "primary"
```

### Cards

```yaml
card-default:
  background: "white"
  border: "1px solid hairline"
  borderRadius: "lg (16px)"
  padding: "24px"
  shadow: "sm"
  hover-shadow: "lg"
  hover-border: "primary/30"

card-eco-light:
  background: "primary-bg (#e6f7f6)"
  border: "1px solid primary-soft"
  borderRadius: "2xl (32px)"
  padding: "32px"
  use: "Eco/sustainability messaging"

card-dark:
  background: "ink-950"
  border: "1px solid rgba(255,255,255,0.1)"
  text: "white"
  borderRadius: "lg"
```

### Service Cards (cinco servicios principales)

```yaml
service-card:
  layout: "vertical with image-top OR horizontal with number-left"
  numbered: true             # "01", "02"... in primary color
  number-font-size: "32px"
  number-font-weight: 800
  title-font: "heading-md"
  description-font: "body-sm muted"
  link-suffix: "Más información →"
  link-color: "primary"
  hover-effect: "Increase shadow, slight scale, arrow translates right"
```

### Hero Section

```yaml
hero:
  variants: ["dark-cinematic", "light-soft", "split-image"]
  default: "split-image"
  layout: "60/40 text-left / image-right"
  pretitle: "label-tiny in primary color"
  headline: "display-xl with gradient option (primary→secondary)"
  subtitle: "body-lg in ink-700"
  cta-stack: "Primary WhatsApp + Secondary outline"
  trust-indicators: "Mini badges below CTAs: years, sedes, certs"
  decorative: "Blob gradients in primary/secondary, blurred 60px"
```

### Stats / Metrics

```yaml
stat-display:
  number: "numerals-display in primary color"
  label: "label-tiny in ink-500"
  layout: "3 to 4 in grid"
  emphasis-card: "Middle card uses primary background with white text"
  pattern: "Numbers grow on scroll-into-view"
```

### Tables (precios, emisiones)

```yaml
table:
  header: "primary background, white text, uppercase tracking-wider"
  row-alternating: "white / ink-50"
  borders: "hairline only"
  prices: "display-lg in primary color"
  reduction-percentages: "display-lg with bold weight"
  rounded: "lg on container"
  shadow: "md"
```

### Top Bar (above main nav)

```yaml
topbar:
  background: "ink-900 OR primary"
  height: "auto, py-2"
  font: "label-tiny"
  contents: "phone + email + hours + WhatsApp link"
  text-color: "white/80"
```

### Floating WhatsApp Button

```yaml
floating-wa:
  position: "fixed bottom-6 right-6"
  size: "56px (w-14 h-14)"
  background: "whatsapp gradient"
  shadow: "glow-whatsapp"
  icon: "WhatsApp logo white"
  animation: "subtle pulse (optional)"
  always-visible: true
  z-index: 50
```

## 📸 Photography & Imagery

### Style guide

- **Cinematic, professional automotive photography**
- **Color grading:** subtle cyan-teal cast in shadows
- **Subjects:** real engines, HHO generators, technicians in cyan polos, clean workshop, family-friendly vehicles
- **NEVER use:** generic businessman handshakes, fake stock smiles, corporate cliché photos

### Image treatments

```yaml
image-treatment:
  rounded: "lg or xl"
  shadow: "lg"
  aspect-ratios: ["square (1:1)", "video (16:9)", "portrait (3:4)"]
  hover: "scale 1.05 over 500ms (gallery cards)"
  overlay-on-dark-hero: "linear-gradient(to right, ink-950 0%, transparent 70%)"
```

### Gallery patterns

- **Process gallery:** 4 vertical images with overlay text "Paso 01/02/03/04"
- **Service grid:** 5-6 cards with image + title + description + arrow link
- **Vehicle types:** 8-grid showing different vehicle categories (sedan, SUV, truck, taxi, moto, fleet, diesel, gasolina)

## ✨ Motion & Interactions

```yaml
transitions:
  default: "all 150ms ease"
  hover-scale: "transform 200ms ease"
  page-fade-in: "opacity 400ms ease-out"

animations:
  pulse-cta: "WhatsApp button pulse, 2s infinite"
  fade-in-up: "On scroll-into-view, 600ms"
  counter-up: "Stats animate from 0, 800ms ease-out"
  parallax-hero: "Subtle image translateY on scroll"

NO use:
  - Bouncing animations
  - Gimmicky page transitions
  - Anything that feels like 2010 marketing
```

## 📱 Responsive

```yaml
breakpoints:
  sm:  "640px"
  md:  "768px"
  lg:  "1024px"
  xl:  "1280px"

mobile-first: true
nav-mobile: "hamburger from md-down"
hero-mobile: "stacked, image hidden or moved below text"
stats-mobile: "2 columns instead of 4"
```

## 🗣️ Voice & Tone

### Content rules

- **Always use** texts verbatim from the original Hydrocell site (never paraphrase)
- **Spanish, Colombian variant** ("camionetas" not "pickups", "Bogotá" not "Bogota")
- **Numbers:** Spanish format ($170.000 not $170,000)
- **WhatsApp number:** +57 314 703 0001 (always with country code)
- **Tagline:** "Mejoramos tu motor, el planeta y tu bolsillo te lo agradecen"

### Headlines style

- ✅ "Devuelve la vida a tu motor con hidrógeno verde"
- ✅ "¿Está sucio tu motor?"
- ✅ "HYDROCELL, Expertos en Descarbonización de Motores"
- ❌ "Revolutionizing engine maintenance" (no anglicismos)
- ❌ Vacíos como "Lo mejor en descarbonización"

### CTAs

- ✅ "Agendar por WhatsApp"
- ✅ "Solicita tu cita"
- ✅ "Quiero descarbonizar"
- ✅ "Contáctanos"
- ❌ "Click here", "Submit", anglicismos

## 🏢 Brand Constants (siempre incluir en footer/contacto)

```yaml
contact:
  primary-whatsapp: "+57 314 703 0001"
  phones:
    - "311 380 9602"
    - "314 703 0001"
    - "323 590 5050"
  hours: "Lunes a Sábado · 8am - 6pm"

sedes:
  - name: "Conquistadores"
    city: "Medellín"
    neighborhood: "Laureles-Estadio"
    address: "Cl. 34 #65C-05"
  - name: "Castilla"
    city: "Medellín"
    neighborhood: "Doce de Octubre"
    address: "Cra. 72b #94-21"
  - name: "Norte de Medellín"
    city: "Medellín"
    neighborhood: "Girardot"
    address: "Cl. 103g #64d-49"
  - name: "Bogotá"
    city: "Bogotá"
    neighborhood: "Galerías"
    address: "Calle 50 #20-48"

certifications:
  - "Patentes norteamericanas"
  - "Certificación Comunidad Económica Europea"
  - "Empresa 100% colombiana"
  - "Desde 2013"
```

## 🎭 Layout Variants (cuál usar según objetivo)

```yaml
F-powerhho:
  use-when: "Premium clean, timeline, eco-conscious audience"
  feature: "Real-time CO₂ counter, timeline 2013→2026"
  hero: "Split image with floating badges"

G-hhoiberica:
  use-when: "Aggressive sales-focused, B2B / partners"
  feature: "Hero slider with bold uppercase claims, testimonial cards"
  hero: "Full-bleed dark with sliding scenes"

H-motortek:
  use-when: "Direct conversion, urban audience"
  feature: "Multiple WhatsApp CTAs (5+), vehicle type gallery"
  hero: "Side-by-side with WhatsApp prominent"

I-flexfuel:
  use-when: "Modern soft brand, lead-generation focus"
  feature: "ROI-oriented metrics, sede search, blog cards"
  hero: "Problem-statement question + diagnostic offer"
```

## 🚀 Quick Reference for Generative AI Tools

When asking Stitch / Claude / v0 / Lovable to build something using this system:

> *"Generate a [page type] for HYDROCELL following the DESIGN.md. Use primary `#00b9b5` and secondary `#4EBD8D`. Inter typography. Reference [variant F/G/H/I] for layout patterns. All CTAs go to WhatsApp +57 314 703 0001. Use texts verbatim from the original Hydrocell content. Include the standard topbar, sticky nav, and floating WhatsApp button."*

### Critical anti-patterns to flag

- ❌ Using stock Tailwind blue/purple instead of `#00b9b5`
- ❌ Generic "Lorem ipsum" or invented content
- ❌ Form-based contact (Hydrocell only uses WhatsApp)
- ❌ Anglicized text or US English content
- ❌ Tech-startup gradients that don't match brand
- ❌ Putting "Hydrocell" lowercase or wrong casing

## 📦 Asset Library Reference

All available images in `/assets/`:

**Hero/Premium:**
- `hero-motor.png` — main engine with cyan hydrogen vapor
- `scanner-diagnostico.png` — HHO generator with bubbles
- `equipo-quienes-somos.jpg` — technicians in workshop

**Services:**
- `analisis-gases-hero.png` — gas analyzer probe
- `limpieza-aceleracion-hero.jpg` — throttle body detail
- `limpieza-aceleracion-detail.jpg` — close-up
- `limpieza-aceleracion-odometro.png` — dashboard 10k km
- `desinfeccion-hero.png` — clean interior with cyan vapor
- `desinfeccion-cojineria.jpg` — upholstery
- `desinfeccion-familia.png` — family entering car

**Vehicles (gallery):**
- `vehicle-sedan.png`, `vehicle-suv.png`, `vehicle-truck.png`
- `vehicle-taxi.png`, `vehicle-motorcycle.png`, `vehicle-fleet.png`

**Quiénes Somos:**
- `quienes-somos-center.jpg`, `quienes-somos-cta.jpg`

**Logo:**
- `logo.png` (cyan version, for light backgrounds)
- `logo-white-on-black.png` (white version, for dark backgrounds)
