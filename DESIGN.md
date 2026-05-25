---
name: Clinical Clarity
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#404752'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#707883'
  outline-variant: '#bfc7d4'
  surface-tint: '#006b5c'
  primary: '#006b5c'
  on-primary: '#ffffff'
  primary-container: '#00a48e'
  on-primary-container: '#003129'
  inverse-primary: '#44ddc1'
  secondary: '#0061a4'
  on-secondary: '#ffffff'
  secondary-container: '#33a0fd'
  on-secondary-container: '#00355c'
  tertiary: '#526069'
  on-tertiary: '#ffffff'
  tertiary-container: '#85949e'
  on-tertiary-container: '#1f2d35'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#68fadd'
  primary-fixed-dim: '#44ddc1'
  on-primary-fixed: '#00201a'
  on-primary-fixed-variant: '#005145'
  secondary-fixed: '#d1e4ff'
  secondary-fixed-dim: '#9ecaff'
  on-secondary-fixed: '#001d36'
  on-secondary-fixed-variant: '#00497d'
  tertiary-fixed: '#d6e5ef'
  tertiary-fixed-dim: '#bac9d3'
  on-tertiary-fixed: '#0f1d25'
  on-tertiary-fixed-variant: '#3b4951'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-lg:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-sm:
    fontFamily: Manrope
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  display-lg-mobile:
    fontFamily: Manrope
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
rounded:
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  unit: 4px
  container-padding: 24px
  stack-gap: 16px
  grid-gutter: 12px
---

## Brand & Style

The brand personality is authoritative yet empathetic, designed to provide patients and practitioners with a sense of calm and precision. The target audience includes health-conscious individuals and patients requiring remote monitoring who value data accuracy without clinical coldness.

The design system utilizes **Glassmorphism** to bridge the gap between high-tech medical equipment and approachable consumer software. By layering frosted surfaces over soft, organic background blurs, the interface feels light and breathable. This aesthetic emphasizes transparency—both visually and metaphorically—ensuring that complex medical data feels accessible and non-threatening. The emotional response should be one of "assisted wellness" rather than "illness tracking."

## Colors

The palette is rooted in medical professionalism, with a focus on vitality and reliability.
- **Primary (#00BFA5):** An Accent Teal representing vitality and "go" states (e.g., healthy heart rate, completed goals).
- **Secondary (#2196F3):** A reliable Medical Blue used for secondary actions, supporting data points, and professional accents.
- **Tertiary (#E3F2FD):** A Soft Blue used for large surface areas and glass tinting to prevent the interface from feeling purely white.
- **Neutral (#F8FAFC):** A clean, cool slate-white used for backgrounds to maintain high legibility.

Backgrounds should use subtle linear gradients of Tertiary to Neutral to provide depth for the glass effect to sit upon.

## Typography

This design system employs **Manrope** for its technical precision and modern, balanced proportions, making it ideal for reading numerical health data. For functional elements like captions and small metadata, **Plus Jakarta Sans** is used to introduce a softer, more approachable feel.

Maintain generous line heights to ensure readability during physical activity. Numerical data (e.g., heart rate, steps) should always use the `display-lg` or `headline-md` tokens to ensure it is the primary focal point of any view.

## Layout & Spacing

The layout follows a **fluid grid** model optimized for small-screen density. On smartwatches, content is centered with a 24px safe-area margin to account for bezel interference.

- **Stacking:** Elements are vertically stacked using a 16px gap to maintain distinct "tap targets."
- **Padding:** Internal card padding is set to a minimum of 16px to ensure content does not touch the highly rounded corners.
- **Micro-spacing:** A 4px base unit governs small adjustments (e.g., space between an icon and its label).

## Elevation & Depth

Depth is achieved through **Glassmorphism** rather than traditional heavy shadows.
1.  **Surface:** The base layer is a soft gradient of Neutral to Tertiary.
2.  **Glass Panels:** UI cards use a 60% opacity white background with a `20px` backdrop blur. 
3.  **Borders:** Each glass panel features a subtle, 1px inner border (top-left weighted) at 40% white opacity to simulate light catching the edge of the "lens."
4.  **Shadows:** Shadows are highly diffused (24px blur), low-opacity (8%), and tinted with the Primary Teal color to create an ambient glow rather than a dark silhouette.

## Shapes

The shape language is defined by extreme roundedness to mimic the organic forms of the human body and the circular hardware of premium smartwatches. 

- **Cards/Containers:** Use `rounded-xl` (48px / 3rem) to create a friendly, "pebble-like" appearance.
- **Buttons:** Always use pill-shaped (fully rounded) geometry to maximize the hit area and maintain the soft aesthetic.
- **Progress Bars:** Use rounded caps for all data visualization strokes to avoid harsh endings.

## Components

### Buttons
Primary buttons use solid Teal (#00BFA5) with white text. Secondary buttons use the glass effect with a subtle blue outline. All buttons must have a minimum height of 48px for easy interaction.

### Health Cards
The core component of the design system. These use the glass effect. Headlines are placed top-left, with the primary metric (e.g., "98 bpm") in the center-right using the `display-lg` token.

### Input Fields
Inputs are pill-shaped with a 10% opacity primary color fill. When focused, the border opacity increases, and a subtle primary glow is applied to the backdrop.

### Data Visualization
Charts should use thick, rounded lines (4px stroke). Use gradients for area charts, transitioning from the Primary color (Teal) at the peak to 0% opacity at the baseline to maintain the "light" feel.

### Status Chips
Small, high-contrast pills used to indicate "Live" tracking or "Syncing" status. These should utilize the Primary color for positive states and a soft coral for warnings.