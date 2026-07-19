---
version: alpha
name: BugZero Design System
description: A clean, corporate IT services and managed support visual language characterized by professional blues, lime-yellow accents, and high-contrast typography.
colors:
  primary: "#00a7e1"
  secondary: "#c8d600"
  surface: "#ffffff"
  background: "#f6f5f2"
  text-primary: "#263238"
  text-secondary: "#52636b"
  accent-light: "#edfaff"
  accent-lime-light: "#f8fae9"
typography:
  headings: "'Pura Std', Arial, sans-serif"
  body: "'Inter', system-ui, sans-serif"
  accent: "'Playfair Display', serif"
spacing:
  section-py: "5rem"
  container-max-w: "112rem"
  gap-standard: "1.75rem"
rounded:
  md: "0.375rem"
  xl: "0.75rem"
  "2xl": "1rem"
  "3xl": "1.5rem"
components:
  button-primary:
    bg: "{colors.primary}"
    text: "#ffffff"
    radius: "{rounded.md}"
    shadow: "0 14px 30px rgba(0,167,225,0.2)"
  card-expertise:
    bg: "variable"
    border: "1px solid"
    radius: "{rounded.2xl}"
---

## Overview
The BugZero visual identity is built around the themes of security, serenity, and professional efficiency. It uses a high-density corporate layout with ample white space, relying on a split palette of deep navy-slate (`#263238`) and electric cyan (`#00a7e1`) contrasted with a lime-green (`#c8d600`) indicator. The tone is reliable and modern, utilizing geometric icons and rounded corner containers to soften technical subject matter.

## Colors
- **Primary Brand**: `#00a7e1` (Cyan) used for action items, headings, and primary brand indicators.
- **Secondary Accent**: `#c8d600` (Lime) used for status indicators (online), step numbers, and high-visibility accents.
- **Text/Deep Neutrals**: `#263238` (Dark Slate) used for primary body text and dark UI backgrounds.
- **Subtle Neutrals**: `#52636b` (Slate Gray) used for secondary descriptive text.
- **Container Backgrounds**:
  - Cyan Tinge: `#edfaff` (15% opacity primary equivalent)
  - Lime Tinge: `#f8fae9` (40% opacity secondary equivalent)
  - Neutral Tinge: `#f4f5f5` (Light gray section backgrounds)

## Typography
- **Headings**: High-impact sans-serif (Pura Std) with tight tracking and a leading of `0.98` for hero statements. Standard weights used are 500 and 600.
- **Body**: Inter is utilized for legibility in paragraphs with `1.25rem` (xl) or `1.125rem` (lg) sizing and relaxed leading (`leading-relaxed`).
- **Systemic Accents**: Playfair Display is present in the CSS for potential serif flourishes, though Inter handles the majority of the UI.
- **Uppercase Labels**: Small text (0.875rem) with high letter-spacing (`0.16em`) paired with a colored square icon for section labeling.

## Layout
- **Grid System**: Utilizes a maximum container width of `112rem`. Page structure transitions from 1-column on mobile to asymmetrical 2-column or 3-column layouts on desktop.
- **Navigation**: High-density horizontal header with 36px (9rem) spacing between links.
- **Section Spacing**: Vertical padding usually ranges between `5rem` (80px) and `6rem` (96px) to define distinct content blocks.

## Elevation & Depth
- **Soft Shadow**: `shadow-sm` and custom cyan glows (`0 14px 30px rgba(0,167,225,0.2)`) are used on primary CTAs.
- **Card Depth**: Cards use a mix of subtle borders (`15%` opacity) and very light background tints rather than heavy drop shadows to maintain a flat, modern aesthetic.
- **Overlays**: Abstract radial gradients (Cyan at 18%, Lime at 34%) are used inside feature containers to create soft depth.

## Shapes
- **Corner Radii**:
  - Small Buttons: `6px` (md)
  - Standard Cards: `16px` (2xl)
  - Large Containers/CTA Blocks: `24px` (3xl)
- **Icon Backgrounds**: Icons are typically encased in `14x14` (size-14) or `12x12` (size-12) rounded-xl or rounded-full containers.

## Components
- **Status Indicator**: A `size-3` square of `{colors.secondary}` used as a prefix for subheadings.
- **Action Buttons**:
  - Primary: Solid `{colors.primary}` with white text and a bottom-weighted shadow.
  - Secondary: Outlined `{colors.primary}` with white background.
- **Expertise Cards**: Large containers with a top-aligned icon, a 24px (2xl) heading, and 18px text.
- **Testimonial Cards**: Vertical flex layouts with a star rating header, large blockquote, and an avatar footer using initials in a circular background.

## Page Sections

### Navigation
A sticky-ready transparent header containing the `bugzero-logo.png` (56px height on desktop). Navigation links use a slate-to-cyan hover transition. A mobile-specific "Contact" button replaces the full menu on small screens.

### Hero Section
Split layout with a text-heavy left column and a graphic right column. Features a 72pt heading with cyan span accents. The right graphic is a complex material composition using a `{rounded.3xl}` border, radial background glows, and a floating "24/7 protected" card component.

### Expertises (Services Grid)
A 3-column responsive grid. Each card uses a different color theme:
- Cloud: Cyan theme (`#edfaff` bg, `#00a7e1` icon).
- Security: Lime theme (`#f8fae9` bg, `#c8d600` icon).
- Support: Dark theme (`#f4f5f5` bg, `#263238` icon).

### Process (How It Works)
A horizontal timeline using large numeric indicators (`01`, `02`, `03`) in primary/secondary colors. Cards are elevated with `shadow-sm` on a neutral gray (`#f4f5f5`) section background.

### Why Us (Value Props)
A 2-column layout. The left side holds the narrative; the right side is a 2x2 grid of small cards with 4px left-hand accent borders matching the specific feature's color theme.

### Testimonials
A 3-column grid of white cards on a light gray background. Includes a 5-star rating system using filled Lucide star icons in lime.

### Final CTA & Footer
A full-width cyan (`#00a7e1`) block with large circular geometric outlines in the corners. The footer below it is minimalist, featuring a top border separator and horizontal link list.

## Motion & Interaction
- **Scroll Reveals**: An `IntersectionObserver` triggers the `animate-on-scroll` class. Components fade in and slide up 30px with a temporary 8px blur filter (`animationIn`).
- **Hovers**: Standard 150ms-200ms transitions on text color and background color for all interactive links and buttons.

## Do's and Don'ts
- **Do**: Use the lime square status indicator for all section labels.
- **Do**: Maintain the specific tight letter-spacing on H1 headings.
- **Don't**: Use sharp corners; almost every container has at least a 12px (xl) radius.
- **Don't**: Overuse the lime-green; it is reserved for accents and status indicators only.

## Accessibility
- **Contrast**: Primary slate text (`#263238`) against white or light gray backgrounds meets WCAG AA standards.
- **Semantic HTML**: Sections are clearly defined with IDs (`#expertises`, `#temoignages`) for fragment navigation.
- **Focus**: Transitions are provided for focusable elements, though explicit focus-ring styles are handled by browser defaults.

## Assets
1. `image: bugzero-logo.png`
2. `other: https://cdn.tailwindcss.com`
3. `other: https://unpkg.com/lucide@latest/dist/umd/lucide.min.js`
4. `embed: https://fonts.googleapis.com`
5. `embed: https://fonts.gstatic.com`
6. `embed: https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Playfair+Display:ital,wght@0,500;1,500&display=swap`
7. `other: https://www.googletagmanager.com/gtag/js?id=G-2M6V79H761`
8. `other: /`
9. `other: /services`
10. `other: /contact`
11. `other: /mentions-legales`
12. `other: /politique-de-confidentialite`

### Exported Codebase Asset Inventory
1. embed: https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&amp;family=Playfair+Display:ital,wght@0,500;1,500&amp;display=swap
   Context: index.html: markup attribute; index.html: absolute url literal
