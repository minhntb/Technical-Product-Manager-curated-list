---
name: Atlassian Design
url: https://atlassian.design/
colors:
  primary: '#1868db'
  primary-hover: '#1558BC'
  primary-pressed: '#144794'
  background: '#ffffff'
  background-dark: '#051524'
  surface: '#ffffff'
  surface-hovered: '#F0F1F2'
  surface-dark: '#1C2B42'
  text-primary: '#292a2e'
  text-secondary: '#505258'
  text-inverse: '#ffffff'
  text-link: '#1868db'
  text-link-hover: '#0065FF'
  text-link-pressed: '#1558BC'
  text-disabled: '#080F214A'
  border: '#dddee1'
  border-focused: '#357DE8'
  accent-lime: '#94c748'
  accent-saffron: '#fca700'
  accent-red: '#f87168'
  accent-discovery: '#af59e1'
  badge-kyah: '#1868db'
  badge-tony: '#af59e1'
  badge-rovo: '#fca700'
typography:
  display:
    family: 'Atlassian Sans'
    size: 68px
    weight: 653
    line-height: 1.2
  heading-h1:
    family: 'Atlassian Sans'
    size: 44px
    weight: 653
    line-height: 1.2
  heading-h2:
    family: 'Atlassian Sans'
    size: 28px
    weight: 653
    line-height: 1.2
  heading-h3:
    family: 'Atlassian Sans'
    size: 24px
    weight: 653
    line-height: 1.2
  body:
    family: 'Atlassian Sans'
    size: 16px
    weight: 400
    line-height: 1.5
  small:
    family: 'Atlassian Sans'
    size: 14px
    weight: 400
    line-height: 1.25
  caption:
    family: 'Atlassian Sans'
    size: 12px
    weight: 400
    line-height: 1.33
  code:
    family: 'Atlassian Mono'
    size: 14px
    weight: 400
    line-height: 1.5
spacing:
  base: 4px
  scale: [0, 4, 8, 12, 16, 20, 24, 32, 40, 48, 80, 128]
radius:
  sm: 2px
  md: 4px
  lg: 8px
  xl: 16px
  xxl: 40px
  full: 9999px
  button: 6px
elevation:
  card: 'rgba(30, 31, 33, 0.25) 0px 1px 1px 0px, rgba(30, 31, 33, 0.31) 0px 0px 1px 0px'
  overlay: 'rgba(0, 0, 0, 0.09) 0px 40px 20px 20px'
  z-negative: -1
  z-interactive: 1
  z-nav: 4
  z-dropdown: 10
  z-tooltip: 20
  z-modal: 100
  z-portal: 600
motion:
  duration-xxshort: '50ms'
  duration-xshort: '100ms'
  duration-short: '150ms'
  duration-medium: '200ms'
  duration-long: '250ms'
  duration-xlong: '400ms'
  duration-xxlong: '600ms'
  duration-dramatic: '800ms'
  easing-in-practical: 'cubic-bezier(0.6, 0, 0.8, 0.6)'
  easing-out-practical: 'cubic-bezier(0.4, 1, 0.6, 1)'
  easing-inout-bold: 'cubic-bezier(0.4, 0, 0, 1)'
  easing-spring: 'linear(0, 0.021, 0.058, 0.107, 0.164, 0.227, 0.292, 0.359, 0.425, 0.49, 0.552, 0.61, 0.664, 0.714, 0.759, 0.8, 0.837, 0.'
components:
  button-primary:
    bg: '{colors.primary}'
    text: '{colors.text-inverse}'
    radius: '{radius.button}'
    padding: '6px 12px'
    font-weight: 500
    font-size: 14px
  button-secondary:
    bg: '{colors.background}'
    text: '{colors.text-secondary}'
    border: '{colors.border}'
    radius: '{radius.button}'
    padding: '6px 12px'
    font-weight: 500
    font-size: 14px
  button-ghost:
    bg: 'transparent'
    text: '{colors.text-secondary}'
    border: 'none'
    radius: '{radius.button}'
    padding: '6px 12px'
    font-weight: 500
    font-size: 14px
  card:
    bg: '{colors.background}'
    radius: '{radius.md}'
    shadow: '{elevation.card}'
  input:
    bg: '{colors.background}'
    border: '{colors.border}'
    radius: '{radius.sm}'
    padding: '8px 12px'
    text: '{colors.text-primary}'
  name-badge:
    bg-kyah: '{colors.badge-kyah}'
    bg-tony: '{colors.badge-tony}'
    bg-rovo: '{colors.badge-rovo}'
    text: '{colors.text-inverse}'
    radius: '{radius.full}'
    padding: '4px 8px'
---

# Design System Inspired by Atlassian Design

## 1. Visual Theme & Atmosphere
Atlassian Design presents a professional and structured visual theme, characterized by a clean white background (`#ffffff`) subtly overlaid with a sparse, light gray dotted grid pattern (inferred from screenshot). The primary brand color is a vibrant blue (`#1868db`), used prominently for interactive elements and key messaging, creating focal points against the otherwise neutral canvas. Typography relies heavily on the `Atlassian Sans` typeface, particularly its `653` weight for display headings, which contributes to a robust and authoritative tone.

The design system emphasizes clarity and usability through generous whitespace, with large sections often separated by 80px or more of vertical padding. Subtle interactive elements are enhanced by CSS animations, such as `transform: scale(1.02)` on hover for certain components, and `opacity 0.3s ease-out` transitions, adding a refined layer of interactivity without being distracting. The overall atmosphere is one of modern efficiency, designed to facilitate complex collaboration tools with a straightforward and engaging user experience.

**Key Characteristics**
- Prominent use of `Atlassian Sans` in `653` weight for headlines.
- Primary blue (`#1868db`) for key interactive elements.
- Generous `80px` vertical spacing between major sections.
- Subtle `transform: scale(1.02)` hover animations on interactive cards.
- Clean white background (`#ffffff`) with a dotted grid pattern.
- Minimalist iconography with clear, geometric forms.
- Name badges use vibrant accent colors like `#af59e1` and `#fca700`.

## 2. Color Palette & Roles
The Atlassian Design color palette is built around a core brand blue, supported by a versatile neutral scale and a set of distinct accent colors for specific semantic uses.

-   **Primary**
    -   **primary** (`#1868db`) — The core brand blue, used for primary calls-to-action, active states, and key brand elements.
    -   **primary-hover** (`#1558BC`) — A darker shade of blue, appearing on hover states for primary interactive elements.
    -   **primary-pressed** (`#144794`) — An even deeper blue, used for active/pressed states of primary interactive components.
-   **Accent Colors**
    -   **accent-lime** (`#94c748`) — A bright green, used for success indicators or positive accents.
    -   **accent-saffron** (`#fca700`) — A warm orange, used for warnings, highlights, or specific brand elements like the "Rovo" badge.
    -   **accent-red** (`#f87168`) — A soft red, likely for danger, error states, or attention-grabbing elements.
    -   **accent-discovery** (`#af59e1`) — A vibrant purple, used for discovery elements or specific brand highlights like the "Tony" badge.
    -   **background-dark** (`#051524`) — A very dark blue, used as a background in specific dark sections or for dark theme surfaces.
-   **Interactive**
    -   **text-link** (`#1868db`) — The default color for hyperlinks, matching the primary brand blue.
    -   **text-link-hover** (`#0065FF`) — A slightly brighter blue for link hover states, ensuring visibility.
    -   **text-link-pressed** (`#1558BC`) — A darker blue for active link states.
-   **Neutral Scale**
    -   **background** (`#ffffff`) — The predominant background color for the overall interface, promoting spaciousness and clarity.
    -   **text-primary** (`#292a2e`) — The primary text color for headings and body copy, offering high contrast on light backgrounds.
    -   **text-secondary** (`#505258`) — A slightly lighter gray for secondary text, labels, or less emphasized content.
    -   **text-inverse** (`#ffffff`) — White text, used on dark backgrounds or colored interactive elements.
    -   **text-disabled** (`#080F214A`) — A muted, semi-transparent dark gray for disabled text, indicating non-interactivity.
-   **Surface & Borders**
    -   **surface** (`#ffffff`) — Default surface color for cards and containers, matching the main background.
    -   **surface-hovered** (`#F0F1F2`) — A very light gray, used for subtle background changes on hoverable surfaces.
    -   **surface-dark** (`#1C2B42`) — A dark blue-gray, serving as a background for components within dark sections or themes.
    -   **border** (`#dddee1`) — A light gray, used for subtle separators, input borders, and outlines.
    -   **border-focused** (`#357DE8`) — A distinct blue, used for focus rings around interactive elements.

## 3. Typography Rules
-   **Font Family**: 'Atlassian Sans', ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Ubuntu, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"; 'Atlassian Mono', SFMono-Regular, Consolas, "Liberation Mono", Menlo, Courier, monospace.
-   **Hierarchy**:
    -   **Display**: 'Atlassian Sans' `68px` `653` · line-height `1.2` · tracking `none` · Used for hero headlines and impactful statements.
    -   **H1**: 'Atlassian Sans' `44px` `653` · line-height `1.2` · tracking `none` · Main section titles.
    -   **H2**: 'Atlassian Sans' `28px` `653` · line-height `1.2` · tracking `none` · Sub-section headings.
    -   **H3**: 'Atlassian Sans' `24px` `653` · line-height `1.2` · tracking `none` · Card titles or prominent subheadings.
    -   **Body**: 'Atlassian Sans' `16px` `400` · line-height `1.5` · tracking `none` · Standard paragraph text for readability.
    -   **Small**: 'Atlassian Sans' `14px` `400` · line-height `1.25` · tracking `none` · Used for auxiliary information and detailed text.
    -   **Caption**: 'Atlassian Sans' `12px` `400` · line-height `1.33` · tracking `none` · Fine print, metadata, or very subtle text.
    -   **Code/Mono**: 'Atlassian Mono' `14px` `400` · line-height `1.5` · tracking `none` · For code snippets and technical content.
-   **Principles**
    -   Hierarchy is established primarily through font size and weight `653`, with `400` reserved for body and supplementary text.
    -   Line heights are relatively tight for headings (1.2) to maintain visual density, while body text uses a more open `1.5` for legibility.
    -   The `Atlassian Sans` family is consistently applied across all textual elements, fostering a unified brand voice.
    -   Monospace font is strictly reserved for code or technical contexts to differentiate it clearly from UI text.
    -   Text color `text-primary` (`#292a2e`) is used for almost all primary content, ensuring high contrast on the `background` (`#ffffff`).

## 4. Component Stylings

### Buttons
Atlassian Design features clear, functional buttons with distinct visual hierarchies and subtle interactive feedback. All buttons use a `6px` border-radius and `14px` font size with `500` weight.

#### Primary Button
A solid blue button for primary actions, providing high contrast and immediate visual prominence. On hover, it darkens slightly, and on press, it darkens further.
```css
.button-primary {
  background-color: var(--color-primary, #1868db);
  color: var(--color-text-inverse, #ffffff);
  font-family: 'Atlassian Sans', ui-sans-serif, system-ui;
  font-size: 14px;
  font-weight: 500;
  padding: 6px 12px;
  border: none;
  border-radius: var(--radius-button, 6px);
  cursor: pointer;
  transition: background-color var(--motion-duration-short, 150ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1));
}

.button-primary:hover {
  background-color: var(--color-primary-hover, #1558BC);
}

.button-primary:active {
  background-color: var(--color-primary-pressed, #144794);
}

.button-primary:disabled {
  background-color: var(--ds-background-disabled, #0515240f); /* inferred from active state */
  color: var(--color-text-disabled, #080F214A); /* inferred from icon disabled */
  cursor: not-allowed;
}
```

#### Secondary Button
A button with a white background and a light gray border, used for secondary actions that need less emphasis than primary actions. It darkens its border and text on hover.
```css
.button-secondary {
  background-color: var(--color-background, #ffffff);
  color: var(--color-text-secondary, #505258);
  font-family: 'Atlassian Sans', ui-sans-serif, system-ui;
  font-size: 14px;
  font-weight: 500;
  padding: 6px 12px;
  border: 1px solid var(--color-border, #dddee1);
  border-radius: var(--radius-button, 6px);
  cursor: pointer;
  transition: background-color var(--motion-duration-short, 150ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1)),
              border-color var(--motion-duration-short, 150ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1)),
              color var(--motion-duration-short, 150ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1));
}

.button-secondary:hover {
  background-color: var(--color-surface-hovered, #F0F1F2); /* inferred from surface hover */
  border-color: var(--color-text-secondary, #505258); /* inferred */
  color: var(--color-text-primary, #292a2e); /* inferred */
}

.button-secondary:active {
  background-color: var(--ds-background-accent-gray-subtle-pressed, #DDDEE1); /* inferred */
  border-color: var(--color-text-primary, #292a2e); /* inferred */
  color: var(--color-text-primary, #292a2e); /* inferred */
}

.button-secondary:disabled {
  background-color: var(--ds-background-disabled, #0515240f); /* inferred */
  color: var(--color-text-disabled, #080F214A); /* inferred */
  border-color: var(--color-border, #dddee1);
  cursor: not-allowed;
}
```

#### Ghost Button
A text-only button with no background or border, ideal for tertiary actions or within navigation. On hover, it gains a subtle background fill and darkens its text.
```css
.button-ghost {
  background-color: transparent;
  color: var(--color-text-secondary, #505258);
  font-family: 'Atlassian Sans', ui-sans-serif, system-ui;
  font-size: 14px;
  font-weight: 500;
  padding: 6px 12px;
  border: none;
  border-radius: var(--radius-button, 6px);
  cursor: pointer;
  transition: background-color var(--motion-duration-short, 150ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1)),
              color var(--motion-duration-short, 150ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1));
}

.button-ghost:hover {
  background-color: var(--color-surface-hovered, #F0F1F2);
  color: var(--color-text-primary, #292a2e);
}

.button-ghost:active {
  background-color: var(--ds-background-accent-gray-subtle-pressed, #DDDEE1); /* inferred */
  color: var(--color-text-primary, #292a2e); /* inferred */
}

.button-ghost:disabled {
  color: var(--color-text-disabled, #080F214A);
  cursor: not-allowed;
}
```

### Cards & Containers
Cards are used to group related content, featuring a clean white background and a subtle shadow. On hover, cards exhibit a slight `scale(1.02)` transform, indicating interactivity.

#### Standard Card
A basic container for content, with a `4px` border-radius and a light shadow for subtle depth.
```css
.card {
  background-color: var(--color-background, #ffffff);
  border-radius: var(--radius-md, 4px);
  box-shadow: var(--elevation-card, rgba(30, 31, 33, 0.25) 0px 1px 1px 0px, rgba(30, 31, 33, 0.31) 0px 0px 1px 0px);
  padding: var(--spacing-24, 24px); /* inferred */
  transition: transform var(--motion-duration-medium, 200ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1));
}

.card:hover {
  transform: scale(1.02);
}
```

### Inputs & Forms

#### Text Input
Standard text input field with a light gray border and `2px` border-radius. On focus, it displays a distinct blue outline.
```css
.text-input {
  background-color: var(--color-background, #ffffff);
  color: var(--color-text-primary, #292a2e);
  font-family: 'Atlassian Sans', ui-sans-serif, system-ui;
  font-size: 16px; /* inferred */
  font-weight: 400; /* inferred */
  padding: 8px 12px;
  border: 1px solid var(--color-border, #dddee1);
  border-radius: var(--radius-sm, 2px);
  transition: border-color var(--motion-duration-short, 150ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1)),
              box-shadow var(--motion-duration-short, 150ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1));
}

.text-input:focus {
  outline: 2px solid var(--color-border-focused, #357DE8);
  outline-offset: 2px;
  border-color: var(--color-border-focused, #357DE8); /* inferred */
}

.text-input:disabled {
  background-color: var(--ds-background-disabled, #0515240f); /* inferred */
  color: var(--color-text-disabled, #080F214A);
  cursor: not-allowed;
}
```

#### Form Label
Labels for form fields, using the primary text color and a slightly smaller font size for clarity.
```css
.form-label {
  color: var(--color-text-primary, #292a2e);
  font-family: 'Atlassian Sans', ui-sans-serif, system-ui;
  font-size: var(--typography-small-size, 14px);
  font-weight: 400;
  margin-bottom: var(--spacing-4, 4px); /* inferred */
  display: block;
}
```

#### Checkbox/Radio
Custom styled checkboxes and radio buttons, typically with a light border and a primary blue fill when checked.
```css
.checkbox-radio {
  appearance: none;
  width: 16px; /* inferred */
  height: 16px; /* inferred */
  border: 1px solid var(--color-border, #dddee1);
  border-radius: var(--radius-sm, 2px); /* Checkbox */
  background-color: var(--color-background, #ffffff);
  cursor: pointer;
  display: inline-block;
  vertical-align: middle;
  transition: background-color var(--motion-duration-xshort, 100ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1)),
              border-color var(--motion-duration-xshort, 100ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1));
}

.checkbox-radio[type="radio"] {
  border-radius: var(--radius-full, 9999px); /* Radio */
}

.checkbox-radio:checked {
  background-color: var(--color-primary, #1868db);
  border-color: var(--color-primary, #1868db);
}

.checkbox-radio:focus {
  outline: 2px solid var(--color-border-focused, #357DE8);
  outline-offset: 2px;
}

.checkbox-radio:disabled {
  background-color: var(--ds-background-disabled, #0515240f); /* inferred */
  border-color: var(--color-border, #dddee1);
  cursor: not-allowed;
}
```

### Navigation

#### Top Navigation Bar
The main navigation bar at the top of the page, providing global access to key sections. It has a subtle shadow for elevation.
```css
.top-nav-bar {
  background-color: var(--color-background, #ffffff);
  box-shadow: var(--elevation-card, rgba(30, 31, 33, 0.25) 0px 1px 1px 0px, rgba(30, 31, 33, 0.31) 0px 0px 1px 0px); /* inferred from z-nav elevation */
  padding: var(--spacing-16, 16px) var(--spacing-32, 32px); /* inferred */
  height: 64px; /* inferred */
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: sticky;
  top: 0;
  z-index: var(--elevation-z-nav, 4);
}
```

#### Navigation Link
Individual links within navigation menus, typically appearing as secondary text. They become primary text on hover and have an active state.
```css
.nav-link {
  color: var(--color-text-secondary, #505258);
  font-family: 'Atlassian Sans', ui-sans-serif, system-ui;
  font-size: var(--typography-small-size, 14px);
  font-weight: 400;
  text-decoration: none;
  padding: var(--spacing-8, 8px) var(--spacing-12, 12px); /* inferred */
  border-radius: var(--radius-sm, 2px); /* inferred */
  transition: color var(--motion-duration-xshort, 100ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1)),
              background-color var(--motion-duration-xshort, 100ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1));
}

.nav-link:hover {
  color: var(--color-text-primary, #292a2e);
  background-color: var(--color-surface-hovered, #F0F1F2);
}

.nav-link.active,
.nav-link[aria-current="page"] {
  color: var(--color-text-primary, #292a2e);
  font-weight: 500; /* inferred */
  background-color: var(--ds-background-accent-blue-subtlest-pressed, #ADCBFB); /* inferred from active pseudoState */
}
```

#### Dropdown Menu
A container for navigation or action items that appears on interaction, typically with a card-like appearance and higher z-index.
```css
.dropdown-menu {
  background-color: var(--color-background, #ffffff);
  border: 1px solid var(--color-border, #dddee1);
  border-radius: var(--radius-md, 4px);
  box-shadow: var(--elevation-card, rgba(30, 31, 33, 0.25) 0px 1px 1px 0px, rgba(30, 31, 33, 0.31) 0px 0px 1px 0px);
  padding: var(--spacing-8, 8px) 0;
  z-index: var(--elevation-z-dropdown, 10);
  min-width: 160px; /* inferred */
  position: absolute; /* inferred */
  transition: opacity var(--motion-duration-short, 150ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1)),
              transform var(--motion-duration-short, 150ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1));
}
```

### Links

#### Standard Link
Default inline text links, using the primary brand blue and an underline. On hover, the color brightens, and on press, it darkens.
```css
.standard-link {
  color: var(--color-text-link, #1868db);
  text-decoration: underline;
  text-decoration-color: var(--color-text-link, #1868db);
  transition: color var(--motion-duration-xshort, 100ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1));
}

.standard-link:hover {
  color: var(--color-text-link-hover, #0065FF);
  text-decoration-color: var(--color-text-link-hover, #0065FF);
}

.standard-link:visited {
  color: var(--color-text-link, #1868db); /* inferred to match default */
}
```

#### Secondary Link
Links that use the secondary text color, typically for less prominent actions or internal navigation within content.
```css
.secondary-link {
  color: var(--color-text-secondary, #505258);
  text-decoration: underline;
  text-decoration-color: var(--color-text-secondary, #505258);
  transition: color var(--motion-duration-xshort, 100ms) var(--motion-easing-out-practical, cubic-bezier(0.4, 1, 0.6, 1));
}

.secondary-link:hover {
  color: var(--color-text-primary, #292a2e); /* inferred to darken slightly */
  text-decoration-color: var(--color-text-primary, #292a2e); /* inferred */
}

.secondary-link:visited {
  color: var(--color-text-secondary, #505258); /* inferred to match default */
}
```

### Badges

#### Name Badge
Small, pill-shaped badges used to highlight names or short labels, featuring a full border-radius and vibrant accent colors.
```css
.name-badge {
  background-color: var(--color-badge-kyah, #1868db); /* Example: Kyah badge */
  color: var(--color-text-inverse, #ffffff);
  font-family: 'Atlassian Sans', ui-sans-serif, system-ui;
  font-size: var(--typography-small-size, 14px);
  font-weight: 500; /* inferred */
  padding: 4px 8px;
  border-radius: var(--radius-full, 9999px);
  display: inline-flex;
  align-items: center;
  gap: var(--spacing-4, 4px); /* inferred */
}

.name-badge.tony {
  background-color: var(--color-badge-tony, #af59e1);
}

.name-badge.rovo {
  background-color: var(--color-badge-rovo, #fca700);
}
```

## 5. Layout Principles
-   **Spacing System**: Atlassian Design utilizes a `4px` base unit for its spacing scale, providing granular control over element separation. The scale includes: `0, 4, 8, 12, 16, 20, 24, 32, 40, 48, 80, 128` pixels.
    -   **Usage Context**:
        -   `4px`: Smallest inline element spacing, icon-to-text.
        -   `8px`: Padding within small components, spacing between form elements.
        -   `12px`: Button padding, spacing between closely related items.
        -   `16px`: Standard component padding, vertical spacing between list items.
        -   `20px`: Moderate spacing for content blocks.
        -   `24px`: Section padding within cards, spacing between distinct components.
        -   `32px`: Larger component spacing, vertical rhythm.
        -   `40px`: Grouping related sections.
        -   `48px`: Significant vertical separation.
        -   `80px`: Major section breaks, hero content padding.
        -   `128px`: Large page margins, horizontal spacing for wide layouts.
-   **Grid & Container** *(Suggested — not measured)*: _Note: container widths and column counts are not extracted from the source. The values below are reasonable defaults inferred from the visible layout density._
    -   **Max Width**: `1280px` for main content areas, ensuring readability on large screens.
    -   **Columns**: A `12-column` grid system, providing flexibility for various content arrangements.
    -   **Gutter**: `24px` between grid columns, maintaining clear separation.
    -   **Section Padding**: `80px` vertical padding for major sections; `128px` horizontal padding on desktop.
-   **Whitespace Philosophy**: Whitespace is a critical element of the Atlassian Design system, used generously to create visual breathing room and emphasize content. Large areas of `background` (`#ffffff`) are intentionally left empty around key components and text blocks, reducing cognitive load and directing user attention. This ample spacing, particularly the `80px` vertical separation for major sections, contributes to a clean, uncluttered, and professional aesthetic.
-   **Border Radius Scale**:
    -   **sm** (`2px`): Subtle rounding for inputs and small interactive elements.
    -   **md** (`4px`): Standard rounding for cards and larger containers.
    -   **lg** (`8px`): Used for more pronounced rounded corners, e.g., larger media elements.
    -   **xl** (`16px`): Larger, softer rounding for distinct UI elements.
    -   **xxl** (`40px`): Very large rounding, potentially for unique visual elements or avatars.
    -   **full** (`9999px`): Pill-shaped elements like badges and avatars.
    -   **button** (`6px`): Specific rounding for interactive buttons, providing a slightly softer edge than `sm`.

## 6. Depth & Elevation
Atlassian Design employs a subtle elevation system to create visual hierarchy and guide user interaction, primarily through shadows and z-index values.

-   **Flat (z-0)**: No shadow — Default state for most background elements and static content.
-   **Interactive (z-negative)**: `z-index: -1` — Used for background elements that might interact with foreground content, like certain layout sections.
-   **Interactive (z-interactive)**: `z-index: 1` · `rgba(30, 31, 33, 0.25) 0px 1px 1px 0px, rgba(30, 31, 33, 0.31) 0px 0px 1px 0px` — Applied to cards and hoverable elements to give them a slight lift and indicate interactivity.
-   **Navigation (z-nav)**: `z-index: 4` · `rgba(30, 31, 33, 0.25) 0px 1px 1px 0px, rgba(30, 31, 33, 0.31) 0px 0px 1px 0px` (inferred) — Used for the top navigation bar to ensure it sits above most content.
-   **Dropdown (z-dropdown)**: `z-index: 10` · `rgba(30, 31, 33, 0.25) 0px 1px 1px 0px, rgba(30, 31, 33, 0.31) 0px 0px 1px 0px` — For dropdown menus and context panels that appear above regular content.
-   **Tooltip (z-tooltip)**: `z-index: 20` — For small, temporary overlays like tooltips.
-   **Modal (z-modal)**: `z-index: 100` — For full-screen or prominent modal dialogs.
-   **Portal (z-portal)**: `z-index: 600` — The highest z-index, reserved for global elements like notification portals or critical alerts.

**Shadow Philosophy**: Shadows are used sparingly and subtly to provide depth without being heavy. The primary `card` shadow (`rgba(30, 31, 33, 0.25) 0px 1px 1px 0px, rgba(30, 31, 33, 0.31) 0px 0px 1px 0px`) creates a gentle lift, enhancing the perception of interactive elements. More pronounced shadows are reserved for transient elements like modals or overlays, ensuring they command attention and visually separate from underlying content.

## 7. Do's and Don'ts

### Do's
-   **Do** use `Atlassian Sans` `653` weight for all headings `H1` through `H3` to maintain a strong typographic hierarchy.
-   **Do** ensure body text in `text-primary` (`#292a2e`) on `background` (`#ffffff`) maintains an AAA contrast ratio of 14.34:1.
-   **Do** apply `80px` vertical spacing between major page sections to ensure ample visual breathing room.
-   **Do** use `primary` (`#1868db`) for the Primary Button background to clearly highlight main calls-to-action.
-   **Do** use `radius.button` (`6px`) for all buttons, and `radius.md` (`4px`) for cards, to maintain consistent corner rounding.
-   **Do** implement a `transform: scale(1.02)` animation on card hover states with `motion-duration-medium` (`200ms`) for subtle interactivity.
-   **Do** use `text-link` (`#1868db`) for standard links, ensuring they are underlined and change to `text-link-hover` (`#0065FF`) on hover.
-   **Do** use `text-secondary` (`#505258`) for secondary navigation links, transitioning to `text-primary` (`#292a2e`) on hover.
-   **Do** use `accent-discovery` (`#af59e1`) for the "Tony" name badge and `accent-saffron` (`#fca700`) for the "Rovo" name badge.

### Don'ts
-   **Don't** use `text-primary` (`#292a2e`) on `background-dark` (`#051524`); the measured contrast ratio of 1.29:1 fails AA standards.
-   **Don't** introduce custom spacing values; adhere strictly to the `4, 8, 12, 16, 20, 24, 32, 40, 48, 80, 128px` spacing scale.
-   **Don't** use `Atlassian Mono` for anything other than code snippets or technical data; it's not intended for general UI text.
-   **Don't** apply shadows to elements with `z-index: 0`; shadows should only be used to indicate elevation or interactivity.
-   **Don't** use `text-secondary` (`#505258`) on `background-dark` (`#051524`); the measured contrast ratio of 2.36:1 fails AA standards.
-   **Don't** use `primary` (`#1868db`) for secondary button backgrounds; reserve it exclusively for primary actions.
-   **Don't** use a border-radius other than `2px` for text inputs; maintain consistency for form elements.
-   **Don't** create custom accent colors for badges; utilize the predefined `accent-lime`, `accent-saffron`, `accent-red`, and `accent-discovery` palette.
-   **Don't** use `font-weight: 653` on body text; reserve this weight for headings to maintain a clear visual hierarchy.

## 8. Responsive Behavior *(Suggested — not measured)*
_Note: breakpoints below are industry-standard recommendations, not measurements from the source. Adjust to the brand's actual media queries when implementing._

-   **Suggested Breakpoints**:
    -   **Mobile Small** (~480px): Typography scales down, horizontal padding reduces to `16px`.
    -   **Mobile Large** (~768px): Cards stack vertically, navigation collapses to a hamburger menu.
    -   **Tablet** (~1024px): Two-column layouts may appear, hero images adjust to fit.
    -   **Desktop** (~1440px): Full desktop layout, main content container width `1280px`.
    -   **Desktop Large** (~1220px + 3.75rem): Wider content