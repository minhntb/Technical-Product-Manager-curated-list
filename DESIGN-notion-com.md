# Design System Inspired by Notion

## 1. Visual Theme & Atmosphere
Notion's design system projects a feeling of structured creativity and approachable power. The aesthetic is built on a foundation of clean, high-contrast typography and a grid-based layout, which speaks to its organizational capabilities. This functional core is softened by a signature illustration style featuring friendly, hand-drawn characters and icons, preventing the tool from feeling sterile. The hero section uses a dark, focused theme (#02093a) with glowing 3D accents to create a dramatic, tech-forward introduction, while the rest of the page is bright, airy, and rendered in a palette of black, white, and subtle off-white surfaces (#f7f7f5).

The overall atmosphere is a duality: it is both a serious productivity tool and a flexible creative space. This is achieved by contrasting the sharp, geometric layout of its UI mockups with organic, colorful illustrations. The use of a custom font, `NotionInter`, ensures typographic crispness from 54px display headings down to 12px captions. Motion is present through an autoplay video in the hero and over 60 distinct CSS keyframe animations (e.g., `fadeIn`, `rotate`) that provide subtle feedback and guide the user's attention without being distracting.

### Key Characteristics
*   **Dual-Tone Experience:** A dramatic, dark-themed hero (#02093a) transitions into a bright, light-themed main content area (#ffffff, #f7f7f5).
*   **Signature Illustrations:** Friendly, colorful, and slightly quirky 3D and 2D illustrations are used to add personality and explain concepts.
*   **Functional Typography:** The entire interface is driven by the `NotionInter` font family, emphasizing clarity and readability at all sizes, from 12px to 54px.
*   **Subtle, Complex Shadows:** Depth is created not with harsh drop shadows, but with soft, multi-layered shadows like `rgba(0, 0, 0, 0.01) 0px 0.175px 1.041px 0px...` to gently lift elements.
*   **Structured Layout:** A strict spacing scale based on multiples of 4px and 8px creates a clean, organized, and predictable rhythm.
*   **Interactive Accents:** Key actions are highlighted with a distinct blue (#097fe8, #62aef0), used for links, primary buttons, and focus states.
*   **Autoplaying Video & CSS Animation:** The design incorporates motion via an autoplaying video in the hero and extensive use of CSS animations for transitions and reveals.

## 2. Color Palette & Roles
The palette is primarily monochrome, relying on black and white for structure and text. A specific shade of blue acts as the primary interactive color, with a set of secondary pastels used for illustrations and accents.

### Primary
*   **Deep Blue (#02093a)** — Used exclusively for the hero section background, creating a focused, immersive introduction.
*   **Action Blue (#097fe8)** — The main interactive color for primary buttons and important links.
*   **Light Blue (#62aef0)** — A lighter variant of the action blue, used for some buttons and accents.

### Accent Colors
*   **Yellow (#ffc95e)** — Used in spot illustrations and UI mockups to draw attention.
*   **Red (#f77463)** — A soft red used for illustrative purposes.
*   **Purple (#ad6ded)** — A muted purple accent found in illustrations.
*   **Dark Blue Accent (#455dd3)** — A secondary blue used in illustrations.

### Neutral Scale
*   **Black (#000000)** — The primary color for all headings and body text.
*   **White (#ffffff)** — The primary background color for the main page content.
*   **Off-White (#f7f7f5)** — A subtle off-white used for card backgrounds and to differentiate sections from the pure white base.
*   **Light Gray (#f6f5f4)** — Used for secondary text on dark backgrounds and as a subtle surface color.
*   **Medium Gray (#615d59)** — Used for secondary body text and captions on light backgrounds.
*   **Light Muted Gray (#a39e98)** — Used for tertiary text, placeholders, and disabled states.

## 3. Typography Rules

### Font Family
*   **Primary:** `NotionInter`, Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"
*   **Serif (Quotes):** `Lyon Text`, Georgia, YuMincho, "Yu Mincho", "Hiragino Mincho ProN", "Hiragino Mincho Pro", "Songti TC", "Songti SC", "SimSun", "PMingLiU", serif
*   **Monospace:** Nitti, Menlo, Courier, monospace

### Hierarchy
| Role | Font | Size | Weight | Line Height | Letter Spacing | Notes |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Display | NotionInter | 54px | 700 | 1.2 | -0.5px | Hero section main headline. |
| H1 | NotionInter | 40px | 700 | 1.25 | -0.5px | Major section titles. |
| H2 | NotionInter | 24px | 700 | 1.3 | -0.25px | Sub-section titles. |
| H3 | NotionInter | 20px | 600 | 1.4 | normal | Card titles and minor headings. |
| Body | NotionInter | 16px | 400 | 1.5 | normal | Main paragraph and component text. |
| Body (Large) | NotionInter | 22px | 400 | 1.5 | normal | Hero subheading/introductory text. |
| Caption | NotionInter | 14px | 400 | 1.4 | normal | Small descriptive text, labels. |
| Quote | Lyon Text | 22px | 400 | 1.6 | normal | Used for customer testimonials. |

### Principles
*   **Clarity First:** The use of `NotionInter` across the board ensures high legibility for UI elements and long-form text.
*   **Strong Weight Contrast:** A clear distinction is maintained between bold `700` weight for headlines and regular `400` weight for body copy, creating an effortless hierarchy.
*   **Purposeful Serif:** The `Lyon Text` serif is reserved exclusively for pull quotes, creating a distinct, more editorial voice for testimonials.
*   **Generous Line Height:** Line heights are consistently generous (1.5 for body), improving readability and contributing to the airy, uncluttered feel.

## 4. Component Stylings

### Buttons
Buttons are designed to be clear and accessible, with distinct styles for different levels of importance.

#### Primary Button
The main call-to-action, used for key conversions like "Get Notion free".

```css
.button-primary {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 10px 16px;
  font-family: 'NotionInter', sans-serif;
  font-size: 16px;
  font-weight: 500;
  color: #ffffff;
  background-color: #097fe8;
  border: 1px solid transparent;
  border-radius: 8px;
  cursor: pointer;
  transition: background-color 0.2s ease;
}

.button-primary:hover {
  background-color: #005bab; /* Derived from --color-button-primary-background-active */
}
```


<details>
<summary>Secondary Button</summary>

Used for secondary actions, often paired with a primary button. It uses an outline style in the hero and a subtle fill on light backgrounds.

```css
.button-secondary {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 10px 16px;
  font-family: 'NotionInter', sans-serif;
  font-size: 16px;
  font-weight: 500;
  color: #000000;
  background-color: #f7f7f5;
  border: 1px solid #e0e0de; /* Inferred */
  border-radius: 8px;
  cursor: pointer;
  transition: background-color 0.2s ease;
}

.button-secondary:hover {
  background-color: #edeceb; /* Inferred */
}
```

</details>

<details>
<summary>Ghost Button</summary>

Used for tertiary actions or within UI components. It appears as a simple text link.

```css
.button-ghost {
  display: inline-flex;
  align-items: center;
  padding: 0;
  font-family: 'NotionInter', sans-serif;
  font-size: 16px;
  font-weight: 500;
  color: #097fe8;
  background-color: transparent;
  border: none;
  cursor: pointer;
  text-decoration: none;
}

.button-ghost:hover {
  text-decoration: underline;
}
```

</details>
### Cards & Containers
Cards are the primary method for grouping related content. They are clean, with soft shadows and rounded corners.

```css
.card {
  background-color: #ffffff;
  border-radius: 12px;
  border: 1px solid rgba(0, 0, 0, 0.07); /* Inferred */
  padding: 24px;
  box-shadow: rgba(0, 0, 0, 0.01) 0px 0.175px 1.041px 0px, rgba(0, 0, 0, 0.02) 0px 0.8px 2.925px 0px, rgba(0, 0, 0, 0.027) 0px 2.025px 7.847px 0px, rgba(0, 0, 0, 0.04) 0px 4px 18px 0px;
  transition: box-shadow 0.2s ease, transform 0.2s ease;
}

.card:hover {
  transform: translateY(-2px);
  box-shadow: rgba(0, 0, 0, 0.01) 0px 1px 3px 0px, rgba(0, 0, 0, 0.02) 0px 3px 7px 0px, rgba(0, 0, 0, 0.02) 0px 7px 15px 0px, rgba(0, 0, 0, 0.04) 0px 14px 28px 0px, rgba(0, 0, 0, 0.05) 0px 23px 52px 0px;
}
```

### Inputs & Forms
Form elements are minimal and clean, with a clear focus state.

```css
.form-label {
  display: block;
  font-family: 'NotionInter', sans-serif;
  font-size: 14px;
  font-weight: 500;
  color: #615d59;
  margin-bottom: 8px;
}

.text-input {
  width: 100%;
  padding: 8px 12px;
  font-family: 'NotionInter', sans-serif;
  font-size: 16px;
  color: #000000;
  background-color: #ffffff;
  border: 1px solid #dfdcd9;
  border-radius: 8px;
  transition: border-color 0.2s ease, box-shadow 0.2s ease;
}

.text-input::placeholder {
  color: #a39e98;
}

.text-input:focus {
  outline: none;
  border-color: transparent;
  box-shadow: rgba(35, 131, 226, 0.57) 0px 0px 0px 1px inset, rgba(35, 131, 226, 0.35) 0px 0px 0px 2px;
}
```

### Navigation
The main navigation bar is context-aware, starting dark and becoming light on scroll.

```css
.nav-bar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 16px 32px;
  position: sticky;
  top: 0;
  z-index: 100;
  background-color: #02093a; /* Initial state in hero */
  color: #f6f5f4;
}

.nav-link {
  font-family: 'NotionInter', sans-serif;
  font-size: 16px;
  font-weight: 400;
  color: #f6f5f4;
  text-decoration: none;
  padding: 8px 12px;
  border-radius: 4px;
  transition: color 0.2s ease, background-color 0.2s ease;
}

.nav-link:hover {
  color: #ffffff;
  background-color: rgba(255, 255, 255, 0.1); /* Inferred */
}
```

### Links

```css
.link {
  color: #097fe8;
  text-decoration: none;
  border-bottom: 1px solid transparent;
  transition: border-color 0.2s ease;
}

.link:hover {
  border-bottom-color: #097fe8;
}

.link-secondary {
  color: #615d59;
  text-decoration: underline;
  text-decoration-thickness: 1px;
}

.link-secondary:hover {
  color: #000000;
}
```

## 5. Layout Principles

### Spacing System
The layout is governed by a consistent spacing scale, derived from a 4px base unit.
*   **Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80 (all in px).

*   **Usage Context:**
    *   **4px:** Micro-spacing, inside small components.
    *   **8px:** Gaps between text and icons, small component padding.
    *   **12px:** Padding for smaller inputs and buttons.
    *   **16px:** Standard component padding, gap between stacked elements.
    *   **24px:** Padding for cards, vertical gap between components.
    *   **32px:** Larger padding, separating distinct content blocks.
    *   **48px:** Gaps between major layout sections.
    *   **64px, 80px:** Vertical padding for entire page sections.

### Grid & Container
The main content resides within a centered container that ensures readability on large screens.
*   **Max Width:** ~1120px
*   **Columns:** 12-column grid for complex layouts, often simplified to 2 or 3 columns.
*   **Gutter:** 24px
*   **Section Padding:** 80px top and bottom for major sections.

### Whitespace Philosophy
Whitespace is used deliberately and generously. It creates a calm, focused reading experience and prevents the dense UI mockups from feeling overwhelming. Ample padding around sections and within cards allows each piece of content to stand on its own.

### Border Radius Scale
*   **4px, 5px:** Small UI elements like tags and minor buttons.
*   **8px:** Standard radius for buttons and inputs.
*   **12px:** Larger radius for cards and containers.
*   **100px, 9999px:** Pill-shaped or fully circular elements.

## 6. Depth & Elevation
Depth is achieved through a sophisticated, multi-layered shadow system and a clear z-index hierarchy.

| Level | Treatment | Use |
| :--- | :--- | :--- |
| z-1 | `z-index: -1;` | Decorative background elements that sit behind content. |
| z-0 (Flat) | `box-shadow: none;` | Base page background, flat text. |
| z-1 (Raised) | `box-shadow: rgba(0, 0, 0, 0.01) 0px 0.175px 1.041px 0px...` | Standard cards, interactive elements on rest. |
| z-2 (Hover) | `box-shadow: rgba(0, 0, 0, 0.01) 0px 1px 3px 0px...` | Hovered cards and active components. |
| z-3 (Sticky) | `z-index: 100;` | Sticky navigation bar. |
| z-4 (Modal) | `z-index: 1000;` | Dropdown menus, popovers. |
| z-5 (Overlay) | `z-index: 2147483647;` | Third-party overlays like consent managers. |

### Shadow Philosophy
Notion's shadows are designed to be felt more than seen. They are composed of multiple, faint layers with different offsets and blurs. This mimics natural lighting and creates a soft, realistic separation between surfaces. The goal is not to create a dramatic "drop" effect but to subtly lift key elements, indicating interactivity and hierarchy.

## 7. Do's and Don'ts

### Do
*   Use `NotionInter` for all UI text, from 12px captions to 54px headlines.
*   Apply an `8px` or `12px` border-radius to all Cards and containers.
*   Use `#000000` for body text on `#ffffff` or `#f7f7f5` backgrounds.
*   Reserve `Lyon Text` exclusively for testimonial quotes.
*   Use the spacing scale for all margins and padding: `8px`, `16px`, `24px`, `32px`.
*   Ensure all interactive elements have a blue focus ring, like the Text Input.
*   Use `#097fe8` for all primary call-to-action Buttons and links.
*   Lift Cards on hover with the z-2 shadow (`rgba(0, 0, 0, 0.01) 0px 1px...`).
*   Keep paragraph text at `16px` with `400` weight for maximum readability.
*   Use `#615d59` for secondary text on light backgrounds.

### Don't
*   Use shadows with harsh, single-layer offsets. Always use the multi-layer shadow strings.
*   Introduce new colors for interactive elements; stick to `#097fe8`.
*   Place text smaller than `16px` on a colored background.
*   Use weights other than `400` or `700` for body copy or major headlines.
*   Apply a border-radius less than `8px` to a main Card container.
*   Use custom spacing values like `10px` or `30px`.
*   Forget to implement the blue `box-shadow` focus state on all Inputs.
*   Use `Lyon Text` for headings or UI labels.
*   Place `#a39e98` text on any background other than `#ffffff`.
*   Use a font size between `24px` and `40px` for headings.

## 8. Responsive Behavior
*Note: The breakpoints below are measured directly from the site's CSS, reflecting its actual responsive implementation.*

### Breakpoints
| Breakpoint Name | Width | Key Changes |
| :--- | :--- | :--- |
| Mobile Small | < 600px | Single-column layout. Typography scales down. Hamburger menu. |
| Mobile Large | 600px+ | Two-column layouts may begin to appear. Increased padding. |
| Tablet | 840px+ | Primary navigation links become visible. Card grids expand to 2-3 columns. |
| Desktop | 1080px+ | Full desktop experience. Max container width is enforced. Complex grids appear. |
| Desktop Large | 1440px+ | Margins and whitespace increase, content width remains constant. |

### Touch Targets
*   All buttons and interactive links should have a minimum tap area of 44x44px.
*   Ensure at least 8px of space between tappable elements to prevent accidental touches.
*   Text inputs should have a height of at least 40px.

### Collapsing Strategy
*   **Navigation:** The top navigation links collapse into a hamburger menu on mobile. The "Get Notion free" CTA remains visible.
*   **Cards:** Multi-column card layouts stack vertically into a single column on screens narrower than 840px.
*   **Typography:** Headline font sizes are reduced on mobile. For example, the 54px Display text may scale down to 40px.
*   **Padding:** Section padding is reduced from 80px to 40px or 32px on mobile to conserve vertical space.
*   **Forms:** Form layouts remain in a single column across all breakpoints for simplicity.

## 9. Agent Prompt Guide

### Quick Color Reference
*   **Primary Background:** `#ffffff`
*   **Hero Background:** `#02093a`
*   **Primary Text:** `#000000`
*   **Secondary Text:** `#615d59`
*   **Primary Action/Link:** `#097fe8`
*   **Card Surface:** `#ffffff` or `#f7f7f5`
*   **Border/Subtle:** `#dfdcd9`

### Iteration Guide
1.  **Typography:** Always use the `NotionInter` font. Headings are `700` weight, body is `400`. Body text is `16px`.
2.  **Spacing:** Use only these values for margin/padding: `4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80` (px).
3.  **Color:** Primary CTAs and links must use `#097fe8`.
4.  **Borders:** Use `8px` or `12px` `border-radius` for all major containers and cards.
5.  **Shadows:** Use the pre-defined multi-layer shadow strings for elevation. Level 1 for static cards, Level 2 for hovered cards.
6.  **Buttons:** Primary buttons have a solid blue (`#097fe8`) background and white text.
7.  **Inputs:** All text inputs must have the blue `box-shadow` focus state.
8.  **Layout:** Content should be in a central container, max-width around `1120px`.
9.  **Mobile:** On screens below `840px`, stack all multi-column layouts vertically.
10. **Contrast:** Body text (`#000000`) always goes on a light background (`#ffffff` or `#f7f7f5`).
11. **Icons:** Pair icons with text where possible; ensure they are friendly and slightly rounded.
12. **Serif Font:** The `Lyon Text` font is only for block quotes/testimonials. Never use it for UI.