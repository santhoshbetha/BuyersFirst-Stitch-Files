---
name: Automotive Negotiation System
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#45464d'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#0058be'
  on-secondary: '#ffffff'
  secondary-container: '#2170e4'
  on-secondary-container: '#fefcff'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#271901'
  on-tertiary-container: '#98805d'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc6ff'
  on-secondary-fixed: '#001a42'
  on-secondary-fixed-variant: '#004395'
  tertiary-fixed: '#fcdeb5'
  tertiary-fixed-dim: '#dec29a'
  on-tertiary-fixed: '#271901'
  on-tertiary-fixed-variant: '#574425'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  headline-sm:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1'
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '600'
    lineHeight: '1.2'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  2xl: 48px
  3xl: 64px
  container-max: 1280px
  gutter: 24px
---

## Brand & Style

The brand personality is rooted in **authority, transparency, and technical precision**. As a platform facilitating high-value automotive negotiations, the UI must feel like a sophisticated financial tool—reliable and unbiased. 

The design style follows a **Modern Corporate** aesthetic with a heavy influence from high-end SaaS patterns (Shadcn/UI). It prioritizes utility and clarity through a minimalist framework, utilizing subtle borders and crisp geometry to organize complex data. The emotional response should be one of "calm control"—reducing the friction of negotiation through structured information architecture and a professional, "high-tech" atmosphere.

## Colors

The palette is designed for high contrast and institutional trust. 
- **Primary (Deep Navy):** Used for typography, headers, and primary structural elements to establish authority.
- **Accent (Electric Blue):** Reserved strictly for primary actions, progress indicators, and interactive states to signify technology and movement.
- **Semantic Colors:** Emerald, Amber, and Rose are used sparingly for status indicators (e.g., "Offer Accepted," "Counter-offer Pending," "Risk Flagged"). 
- **Surface Colors:** A base of clean white (#FFFFFF) is layered over a Soft Slate (#F8FAFC) background to create subtle depth through containerization.

## Typography

**Inter** is the sole typeface for this design system, chosen for its exceptional legibility in data-dense environments. 

- **Hierarchy:** Use semi-bold and bold weights for numerical values and deal terms to ensure they are the first thing a user sees. 
- **Readability:** Body text uses a generous 1.5 line height to prevent fatigue during long reading sessions of contract terms.
- **Labels:** Use the `label-md` style for table headers and small metadata tags to differentiate secondary information from primary content.

## Layout & Spacing

The system employs a **Fixed Grid** approach for desktop views to maintain a controlled, professional document feel, while transitioning to a **Fluid Grid** for mobile.

- **Grid:** A 12-column grid system is used for dashboard layouts.
- **Spacing Rhythm:** Based on a 4px scale. Use `md` (16px) for internal card padding and `lg` (24px) for spacing between major sections.
- **Mobile Adaptivity:** On mobile, margins reduce to 16px and multi-column forms collapse into a single-column stack to prioritize readability of pricing and terms.

## Elevation & Depth

Depth is achieved through **Low-contrast outlines** and **Tonal Layers** rather than heavy shadows.

- **Borders:** Use 1px borders in Slate-200 (#E2E8F0) to define containers. This provides a "blueprint" feel that suggests precision.
- **Shadows:** Use a single, very soft "ambient" shadow for primary floating elements (like modals or dropdowns).
  - *Example:* `0px 1px 3px rgba(15, 23, 42, 0.1), 0px 1px 2px rgba(15, 23, 42, 0.06)`
- **Surfaces:** Use high-contrast white containers against the soft slate background to pull the user's attention to the data.

## Shapes

The design system utilizes **Soft** geometry. 
- **Base Corner Radius:** 0.25rem (4px) for smaller components like checkboxes and small buttons.
- **Large Components:** Cards and main content containers use `rounded-lg` (8px) to feel modern but still disciplined.
- **Pills:** Avoid fully rounded pills except for status tags (e.g., "Active"), which helps them stand out as metadata.

## Components

- **Buttons:** Primary buttons use the Deep Navy background with white text. Secondary actions use the Electric Blue as a text color with a 1px border.
- **Input Fields:** Use 1px Slate-200 borders. On focus, the border transitions to Electric Blue with a subtle 2px outer glow.
- **Cards:** White background, 1px Slate-200 border, and `rounded-lg` corners. Headers within cards should have a subtle bottom border.
- **Negotiation Chips:** Use high-contrast badges for "Current Offer," "Target Price," and "Gap." These should be the most visually distinct elements on the page.
- **Data Tables:** Stripeless. Use subtle hover states (#F1F5F9) and clear dividers. Ensure numerical data is monospaced or uses tabular lining for easy comparison.
- **Progress Steppers:** Use a linear, minimalist stepper at the top of negotiation flows to provide a sense of transparency and "distance to finish."