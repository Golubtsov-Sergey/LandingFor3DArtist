---
name: Architectural Narrative
colors:
  surface: '#f9f9f9'
  surface-dim: '#dadada'
  surface-bright: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f3'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1a1c1c'
  on-surface-variant: '#444748'
  inverse-surface: '#2f3131'
  inverse-on-surface: '#f1f1f1'
  outline: '#747878'
  outline-variant: '#c4c7c7'
  surface-tint: '#5f5e5e'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#1c1b1b'
  on-primary-container: '#858383'
  inverse-primary: '#c8c6c5'
  secondary: '#5e5e5e'
  on-secondary: '#ffffff'
  secondary-container: '#e3e2e2'
  on-secondary-container: '#646464'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#1a1c1c'
  on-tertiary-container: '#838484'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e5e2e1'
  primary-fixed-dim: '#c8c6c5'
  on-primary-fixed: '#1c1b1b'
  on-primary-fixed-variant: '#474746'
  secondary-fixed: '#e3e2e2'
  secondary-fixed-dim: '#c7c6c6'
  on-secondary-fixed: '#1b1c1c'
  on-secondary-fixed-variant: '#464747'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1a1c1c'
  on-tertiary-fixed-variant: '#454747'
  background: '#f9f9f9'
  on-background: '#1a1c1c'
  surface-variant: '#e2e2e2'
typography:
  display-lg:
    fontFamily: Playfair Display
    fontSize: 72px
    fontWeight: '400'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-sm:
    fontFamily: Playfair Display
    fontSize: 48px
    fontWeight: '400'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '400'
    lineHeight: '1.3'
  headline-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 28px
    fontWeight: '400'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.0'
    letterSpacing: 0.1em
  caption:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.4'
spacing:
  margin-desktop: 80px
  margin-tablet: 40px
  margin-mobile: 24px
  gutter: 24px
  section-gap: 160px
  stack-sm: 8px
  stack-md: 24px
  stack-lg: 48px
---

## Brand & Style

This design system is built for high-end architectural visualization, where the UI serves as a silent, sophisticated frame for the imagery. The brand personality is **quietly authoritative, precise, and atmospheric**. It draws heavily from European editorial design and minimalism, prioritizing negative space and structural balance over decorative elements.

The emotional response should be one of **calm and prestige**. By utilizing a "Gallery Effect"—where the interface recedes to let the "materiality" of the renders take center stage—the design system communicates a premium, studio-grade professionalism. It avoids trends in favor of timeless, grid-based layouts that reflect the geometric rigor of architecture itself.

## Colors

The palette is strictly monochromatic and neutral to ensure it never competes with the colors in the architectural visualizations. 

- **Primary (#1A1A1A):** A deep charcoal, used for primary typography and structural lines. It provides high-contrast legibility without the harshness of pure black.
- **Secondary (#757575):** A soft grey for metadata, labels, and secondary information.
- **Tertiary/Neutral (#F9F9F9, #EAEAEA):** These off-whites and light greys create "air" in the design. Use #F9F9F9 for the main canvas to reduce eye strain compared to pure white, and #EAEAEA for subtle borders and dividers.

## Typography

Typography is the primary vehicle for elegance in this design system. 

- **Playfair Display** is used for all major headings. It should be typeset with generous leading and occasional use of italics for emphasis. Large display sizes should use tighter letter spacing to feel "locked" and intentional.
- **Inter** provides a clean, functional counterpoint. It is used for all body text and UI labels to maintain a contemporary studio feel. 
- **Label-caps** is a specific utility role for navigation and project categories, using high tracking (letter spacing) to evoke a sense of high-end branding.

## Layout & Spacing

The layout follows a **Fixed Grid** philosophy with asymmetric editorial tendencies. 

- **The Grid:** Use a 12-column grid for desktop. Images should frequently "break" the expected symmetry—for example, a hero image might span 8 columns, leaving 4 columns of white space for a caption or simply to let the layout breathe.
- **Section Gaps:** Use an aggressive 160px vertical gap between major project sections to signify a clear change in narrative.
- **Margins:** Large external margins (80px on desktop) act as a matte for the content, framing the portfolio like a physical book.

## Elevation & Depth

To maintain the minimalist aesthetic, this design system eschews shadows and traditional depth. 

- **Tonal Layering:** Depth is achieved by placing elements on slightly different neutral backgrounds (e.g., a #FFFFFF card on a #F9F9F9 background).
- **Subtle Outlines:** Use 1px solid borders in #EAEAEA to define boundaries for tables or input fields. These should feel like hairline strokes from a technical drawing.
- **Glassmorphism:** Navigation bars may use a subtle backdrop blur (20px) with a semi-transparent white tint to maintain visibility over high-detail architectural renders while scrolling.

## Shapes

The shape language is strictly **Sharp (0)**. 

Architectural visualization is a discipline of precision, corners, and structural integrity. All buttons, images, and container elements must have 0px border radii. This reinforces the "architectural" feeling and aligns with classic European editorial layouts. Circular elements should only be used for functional icons or specific decorative flourishes to contrast the pervasive rectangularity.

## Components

- **Project Cards:** Large, portrait-oriented containers (4:5 or 3:4 ratio). Titles appear in `headline-lg` below the image, accompanied by `label-caps` for the year or location. Use a slight opacity fade on hover for the image.
- **Buttons:** Primary buttons are text-based with a 1px bottom border (underline). On hover, the border width increases or the text shifts slightly. No "box" buttons unless for critical CTAs, which should be solid charcoal with white text.
- **Data Tables:** Used for project specs (Client, Location, Materials). Use `label-caps` for headers and `body-md` for data. Borders should only be horizontal, using #EAEAEA.
- **Input Fields:** Minimalist underlines rather than boxes. Focus states transition the underline from #EAEAEA to #1A1A1A.
- **Navigation:** A minimalist top bar or a "hamburger" that opens a full-screen overlay. The full-screen menu should use `display-sm` for links, centered with significant vertical spacing.
- **Image Captions:** Typeset in `caption`, aligned to the right or left of images to create an asymmetric, "noted" look.