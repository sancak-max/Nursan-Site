---
name: Industrial Intelligence System
colors:
  surface: '#faf9fd'
  surface-dim: '#dbd9dd'
  surface-bright: '#faf9fd'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f4f3f7'
  surface-container: '#efedf1'
  surface-container-high: '#e9e7eb'
  surface-container-highest: '#e3e2e6'
  on-surface: '#1a1b1e'
  on-surface-variant: '#414754'
  inverse-surface: '#2f3033'
  inverse-on-surface: '#f1f0f4'
  outline: '#727785'
  outline-variant: '#c1c6d6'
  surface-tint: '#005bc0'
  primary: '#005bbf'
  on-primary: '#ffffff'
  primary-container: '#1a73e8'
  on-primary-container: '#ffffff'
  inverse-primary: '#adc7ff'
  secondary: '#8e4e00'
  on-secondary: '#ffffff'
  secondary-container: '#fc941f'
  on-secondary-container: '#643600'
  tertiary: '#9e4300'
  on-tertiary: '#ffffff'
  tertiary-container: '#c55500'
  on-tertiary-container: '#0e0200'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc7ff'
  on-primary-fixed: '#001a41'
  on-primary-fixed-variant: '#004493'
  secondary-fixed: '#ffdcc1'
  secondary-fixed-dim: '#ffb878'
  on-secondary-fixed: '#2e1500'
  on-secondary-fixed-variant: '#6c3a00'
  tertiary-fixed: '#ffdbcb'
  tertiary-fixed-dim: '#ffb691'
  on-tertiary-fixed: '#341100'
  on-tertiary-fixed-variant: '#783100'
  background: '#faf9fd'
  on-background: '#1a1b1e'
  surface-variant: '#e3e2e6'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: '600'
    lineHeight: 44px
    letterSpacing: -0.02em
  metric-xl:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '500'
    lineHeight: 34px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 24px
    letterSpacing: '0'
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
    letterSpacing: '0'
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
    letterSpacing: '0'
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  data-table:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 20px
    letterSpacing: '0'
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
  gutter: 16px
  margin: 24px
---

## Brand & Style

This design system establishes a high-performance, analytical environment for ZFS Madencilik. It merges the utility-focused precision of a modern industrial operation with the sophisticated data density of enterprise advertising platforms. The visual language is **Corporate / Modern**, characterized by exceptional clarity, a strict structural grid, and an "industrial-digital" aesthetic. 

The UI should evoke a sense of controlled power and real-time accuracy. By utilizing high-density layouts and a neutral background, we prioritize data visibility over decorative elements. The interface remains quiet until action or attention is required, at which point focused color accents guide the user's eye to critical operational metrics and safety alerts.

## Colors

The palette is optimized for long-duration monitoring and rapid data synthesis. The **White background** provides a sterile, high-contrast canvas that minimizes eye strain. **Primary Blue (#1a73e8)** is reserved strictly for interactive elements, navigation states, and primary success metrics, mirroring the authoritative feel of Google's professional tools.

**Safety Orange (#f8911b)** serves as the high-priority signal color, used exclusively for system alerts, production highlights, and items requiring immediate intervention. Neutral tones are tiered: **Dark Gray (#202124)** for primary legibility and a softer gray for secondary metadata. Borders and dividers utilize a subtle cool gray to maintain structure without creating visual noise.

## Typography

The design system utilizes **Inter** to achieve a systematic, utilitarian feel that excels in high-density data environments. The type scale is intentionally compact to allow for maximum information density on a single screen without sacrificing legibility.

Headlines use a medium weight for clear hierarchy, while large metrics utilize a slightly tighter letter-spacing to appear as a singular visual unit. Labels for data tables and small captions use an uppercase style with increased tracking to differentiate "metadata" from "content." Use tabular font features for all numeric data to ensure that columns of figures align perfectly for easy comparison.

## Layout & Spacing

This design system employs a **Fixed grid** philosophy for the main dashboard containers to ensure consistent scanability across desktop displays. A 12-column grid is used for the dashboard layout, with a 16px gutter between cards. 

Spacing follows a strict 4px base unit. Metric cards and data tables should prioritize density; vertical padding in table rows is kept to a minimum (8px) to maximize the number of visible rows. Content is grouped into logical modules (cards) that sit on the grid, creating a "tiled" industrial dashboard appearance.

## Elevation & Depth

To maintain a "digital-first" industrial look, the design system avoids heavy shadows in favor of **low-contrast outlines** and **tonal layers**. 

Most containers are flat with a 1px border (#dadce0). Elevation is reserved for interactive states:
- **Level 0 (Base):** Main background (#ffffff).
- **Level 1 (Cards):** 1px border, no shadow. Used for metric cards and tables.
- **Level 2 (Hover/Active):** A subtle, highly diffused shadow (0px 4px 12px rgba(0,0,0,0.08)) is applied when a card is interactive or hovered.
- **Level 3 (Overlays):** Modals and dropdowns use a crisp 1px border plus a medium-intensity shadow to separate them from the dense background data.

## Shapes

The shape language is **Soft (0.25rem)**. This subtle rounding provides a modern, approachable feel while maintaining the rigid, professional structure required for an industrial mining dashboard. 

Buttons, input fields, and metric cards all share this 4px corner radius. This uniformity reinforces the "modular" nature of the design system. Avoid pill-shaped elements except for status chips, where the distinct shape helps them stand out from the rectangular grid of the data tables.

## Components

### Buttons & Inputs
Primary buttons use a solid blue background (#1a73e8) with white text and 4px rounded corners. Secondary buttons use a 1px gray border with blue text. Input fields should have a 1px border and a subtle gray background on hover to indicate interactivity.

### Metric Cards
Each card features a label (top-left), the primary metric in `metric-xl` (center-left), and a trend indicator (bottom-right). Trend indicators use Green (#1e8e3e) for positive growth and Red (#d93025) for negative, paired with a small directional arrow.

### High-Density Data Tables
Rows are 40px in height with 1px bottom borders. Headers are sticky, using a light gray background (#f8f9fa) and `label-caps` typography. Cells containing "Safety Alerts" or "Critical Errors" should use a subtle orange tint (#fff4e5) for the entire row to ensure high visibility.

### Performance Charts
Charts should use clean lines without area fills unless specifically needed for volume visualization. Use the Primary Blue for the main data line and Safety Orange for threshold lines or targets. Grid lines within charts should be faint (1px, #f1f3f4).

### Status Chips
Small, 20px height indicators with light background tints and dark text (e.g., "Active" in a light green chip, "Maintenance" in a light orange chip). These help users scan tables for operational status rapidly.