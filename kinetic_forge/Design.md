---
name: Kinetic Forge
colors:
  surface: '#101418'
  surface-dim: '#101418'
  surface-bright: '#36393f'
  surface-container-lowest: '#0b0e13'
  surface-container-low: '#191c21'
  surface-container: '#1d2025'
  surface-container-high: '#272a2f'
  surface-container-highest: '#32353a'
  on-surface: '#e1e2e9'
  on-surface-variant: '#d8c3ad'
  inverse-surface: '#e1e2e9'
  inverse-on-surface: '#2e3036'
  outline: '#a08e7a'
  outline-variant: '#534434'
  surface-tint: '#ffb95f'
  primary: '#ffc174'
  on-primary: '#472a00'
  primary-container: '#f59e0b'
  on-primary-container: '#613b00'
  inverse-primary: '#855300'
  secondary: '#ffb3ad'
  on-secondary: '#68000a'
  secondary-container: '#a40217'
  on-secondary-container: '#ffaea8'
  tertiary: '#56e5a9'
  on-tertiary: '#003824'
  tertiary-container: '#30c88f'
  on-tertiary-container: '#004e34'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffddb8'
  primary-fixed-dim: '#ffb95f'
  on-primary-fixed: '#2a1700'
  on-primary-fixed-variant: '#653e00'
  secondary-fixed: '#ffdad7'
  secondary-fixed-dim: '#ffb3ad'
  on-secondary-fixed: '#410004'
  on-secondary-fixed-variant: '#930013'
  tertiary-fixed: '#6ffbbe'
  tertiary-fixed-dim: '#4edea3'
  on-tertiary-fixed: '#002113'
  on-tertiary-fixed-variant: '#005236'
  background: '#101418'
  on-background: '#e1e2e9'
  surface-variant: '#32353a'
typography:
  display-lg:
    fontFamily: Chivo
    fontSize: 48px
    fontWeight: '900'
    lineHeight: 52px
  display-lg-mobile:
    fontFamily: Chivo
    fontSize: 32px
    fontWeight: '900'
    lineHeight: 36px
  headline-lg:
    fontFamily: Chivo
    fontSize: 28px
    fontWeight: '800'
    lineHeight: 34px
  headline-md:
    fontFamily: Chivo
    fontSize: 22px
    fontWeight: '700'
    lineHeight: 28px
  headline-sm:
    fontFamily: Chivo
    fontSize: 18px
    fontWeight: '700'
    lineHeight: 24px
  body-lg:
    fontFamily: Chivo
    fontSize: 16px
    fontWeight: '500'
    lineHeight: 24px
  body-md:
    fontFamily: Chivo
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-lg:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '700'
    lineHeight: 18px
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 10px
    fontWeight: '600'
    lineHeight: 14px
  telemetry-counter:
    fontFamily: JetBrains Mono
    fontSize: 36px
    fontWeight: '800'
    lineHeight: 40px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  gutter: 1.5rem
  gutter-mobile: 0.75rem
  margin: 2rem
  margin-mobile: 1rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2.5rem
---

## Brand & Style

This design system is engineered specifically for harsh, high-throughput manufacturing environments, ruggedized touchscreen terminals, overhead Andon display boards, and operator control stations. 

The aesthetic merges **Tactile Industrial Precision** with **Functional High-Contrast Utility**. It prioritizes instant optical recognition over decorative minimalism, eliminating ambiguity during line stoppages, mechanical faults, and critical safety thresholds. 

### Key Characteristics
- **Grounded Durability:** Deep carbon and basalt surfaces replicate powder-coated industrial chassis, reducing optical glare under harsh sodium-vapor or high-bay LED lighting.
- **Physicality & Tactility:** Deep inset bevels, extruded mechanical switches, and segmented indicator banks designed to feel like physical DIN-rail and NEMA-rated hardware.
- **Emergency Clarity:** High-visibility signaling colors mapped directly to industrial safety protocols (amber caution, operational green, and critical stop red).
- **Legibility at Distance:** High contrast ratios (exceeding WCAG AAA where possible) to maintain readability from 3–5 meters across active plant floors and while wearing tinted protective eyewear.

## Colors

The palette operates under a strict dark industrial framework designed for terminal screens and plant displays. Tonal layering keeps background luminance low while state colors command direct visual hierarchy.

### Functional Palette Structure
- **Carbon Baseline (Neutral):** `#12151A` forms the canvas. Containers elevate sequentially through `#1A1F26` (surface container) up to `#242B35` (surface active/hover), simulating textured anodized aluminum and heavy-gauge plastic enclosures.
- **Hazard Amber (Primary):** `#F59E0B` signals warnings, active line overrides, production throttling, and primary calls-to-action requiring operator acknowledgment.
- **Emergency Red (Secondary):** `#EF4444` is reserved solely for critical Andon alarm triggers, emergency stops (E-Stop), safety zone breaches, and unacknowledged failure states.
- **Operational Jade (Tertiary):** `#10B981` denotes nominal operations, active line tempo, calibrated sensors, and steady-state telemetry.
- **Signal White & Cool Grey (Content):** Pure text scales from `#F8FAFC` (100% white-amber tinted for high-stress reading) down to `#64748B` for secondary equipment metadata and serial tags.

Never use pure black (`#000000`) for surfaces, as it flattens the layered physical depth required for tactile shopfloor interactions.

## Typography

Typography balances rapid scanning and numerical fidelity. Two typefaces drive the system: **Chivo** for high-impact structural communication, and **JetBrains Mono** for all industrial metrics, line telemetry, timestamps, and error codes.

### Hierarchy & Role Rules
- **Structural Text (Chivo):** Heavy geometric weights (`700` to `900`) provide authoritative headlines that resist visual degradation under angled terminal perspective distortion.
- **Technical & Numeric Data (JetBrains Mono):** Standardized tabular figures prevent layout shift when numeric counters, tact-time trackers, and temperature telemetry tick upwards or fluctuate rapidly.
- **Labels & Badges:** Monospace micro-copy is always set in uppercase with slight tracking (+0.05em) to maintain crisp character separation on low-DPI industrial capacitive touch displays.

## Layout & Spacing

The layout is grounded in a **Fluid Grid with Hard Safety Bounds**. Plant terminals range from rugged 10-inch tablets to 65-inch overhead station monitors, requiring strict mechanical modularity.

### Layout Philosophy
- **Standard Desktop & Large Terminal Displays (≥1024px):** 12-column dynamic grid with a generous `1.5rem` (`24px`) gutter. This maintains separation between machine zones and prevents accidental touch inputs when operators wear heavy protective gloves.
- **Mobile & Handheld Diagnostic Units (<1024px):** Reflows down to a 4-column stack. Gutters compress to `0.75rem` (`12px`), while outer margins contract to `1rem` to maximize actionable screen space.
- **Touch Target Density:** Any actionable element must honor an absolute minimum interactive area of `48px x 48px` (ideally `56px` minimum for critical station triggers). Spacing between interactive surfaces never dips below `space-sm` (`8px`) to eliminate fat-finger errors during high-stress operational adjustments.

## Elevation & Depth

Visual hierarchy uses **Physical Insetting, Mechanical Shadowing, and Tonal Relief** instead of soft ambient diffusion. Surfaces mimic machined metal plates and sunken equipment panels.

### Surface Tiers
1. **Base Chassis (Level 0):** Pure background `#12151A`. Recessed, non-interactive foundation.
2. **Terminal Bays & Cards (Level 1):** Background `#1A1F26` with a crisp `1px` inner structural border of `#2D3748`. Supported by a hard drop shadow (`0 2px 0 0 #0B0D11, 0 4px 12px rgba(0, 0, 0, 0.6)`) to project forward from the machine housing.
3. **Interactive Buttons & Selectors (Level 2):** Raised elements built with a simulated top-edge bevel (1px solid `#3E4C5E` top, 2px solid `#000000` bottom) giving tangible physical thickness.
4. **Alarm Overlay & Modal States (Level 3):** Floats above the interface with a hard outline matching the alarm state (e.g., `2px solid #EF4444`) accompanied by an ambient peripheral red or amber glow blur (`0 0 24px rgba(239, 68, 68, 0.35)`).

### Active Depressed States
When an operator interacts with touchscreens, interactive controls shift `2px` downward and replace bottom shadow offsets with a sunken dark inner shadow (`inset 0 2px 4px rgba(0, 0, 0, 0.8)`), confirming mechanical actuation.

## Shapes

The design uses a **Soft (Level 1)** industrial curvature schema (`4px` base radius). 

Excessive rounding reads as consumer-grade and reduces available display real estate; zero-radius sharp edges create optical fatigue on dark matrices. A `4px` baseline radius mimics stamped sheet metal or injection-molded casings, softening corners while preserving a disciplined, utilitarian architecture.

- **Standard Components (Buttons, Inputs, Cards):** `0.25rem` (`4px`).
- **Compound Modules (Station Enclosures, Terminal Bays):** `0.5rem` (`8px`) using `rounded-lg`.
- **Status Pills & LED Indicators:** Full pill (`9999px`) reserved strictly for circular hardware LED indicators, run lights, and machine mode toggles.

## Components

### Buttons & Actuators
- **Primary Industrial Push:** Heavyweight `#F59E0B` background with `#000000` text, bold `Chivo` typography. Hard bottom edge border (`2px solid #B45309`). On tap, compresses down by 2px with an inner shadow.
- **E-Stop & Danger Action:** Dual-tone diagonal safety hazard stripes (`45deg` repeating stripes of `#EF4444` and `#991B1B` at `12px` intervals) framing a central high-visibility action text block. 
- **Secondary Acknowledge:** Outlined dark button with `1.5px` border in `#475569`, surface filled with `#1E293B`, crisp white text.

### Alert Status Badges & Andon Indicators
- **Tri-State Pillar Indicators:** Stacked vertical micro-blocks representing standard manufacturing Andon lights (Red / Amber / Green). Inactive states are dimmed to 20% opacity; active states feature solid fills and a calibrated luminance halo.
- **Fault Badges:** Monospace `JetBrains Mono` label badges, bordered in `1px` high-contrast color lines with a 15% color-matched background tint.

### Industrial Cards & Machine Bays
- Rigid card structures framed by a `#2D3748` technical border.
- Headers are visually partitioned using a solid micro-groove horizontal separator (`1px solid #242B35`), containing machine identifier tags, station numbers, and a top-right status dot.

### Lists & Telemetry Logs
- Alternating row banding using `#161B22` and `#1A1F26` to keep dense maintenance logs legible.
- Strict column grid alignment with right-aligned numeric data and left-aligned machine sensor designations.
- Timestamp elements fixed to JetBrains Mono with 80% opacity neutral text.

### Inputs, Sliders & Selectors
- Recessed input boxes (`#0E1116` interior background) with high-contrast active borders (`#F59E0B`). Minimum height of `48px` to facilitate thumb control without stylus gear.
- Checkboxes and toggles modeled after mechanical industrial toggle switches, featuring prominent ON/OFF position contrast and audible/haptic feedback integration where terminals permit.
