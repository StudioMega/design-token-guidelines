# Mega Design Token Guidelines

Design tokens are standardized, reusable variables that store design decisions, such as colors, fonts, spacing, and other visual elements. These tokens help maintain consistency across a design system by ensuring that these elements are applied uniformly across different platforms and devices.

## Table Of Contents

- [Why Use Design Tokens?](#why-use-design-tokens)
- [Design Token Naming](#design-token-naming)
- [Colors](#colors)
- [Fonts](#fonts)
- [Spacing](#spacing)
- [Animation](#animation)
- [Border](#border)
- [Sizing](#sizing)
- [Other Stuff](#other-stuff)

## Why Use Design Tokens?

- **Consistency:** They ensure a cohesive visual identity by standardizing design elements across different components and platforms.
- **Efficiency:** They allow designers and developers to make updates quickly. Changing a token value, like a color or font size, will automatically update all instances where the token is used.
- **Scalability:** As projects grow, design tokens help manage complexity by centralizing design decisions, making it easier to maintain and evolve the design system.
- **Collaboration:** They bridge the gap between design and development, providing a common language and making it easier for teams to work together.
- **Adaptability:** Tokens can be adapted to different themes or modes (e.g., light and dark mode) without needing to redesign or recode elements from scratch.

## Design Token Naming

Design tokens should have intuitive and descriptive names that clearly indicate their purpose. To ensure consistency and clarity, we follow these naming guidelines:

- **Naming Structure:** Use the format `{category}-{role}-{variant}-{modifier}`.
- **Category:** Always include a category, such as color, space, font, or button.
- **Role:** Define the role, such as background, size, or radius, using a consistent set of terms.
- **Variant:** Optionally include a variant, such as muted, inverse, or error. Omit this if not applicable.
- **Modifier:** Optionally include a state modifier, like hover, active, or focus. Omit if not needed.
- **Avoid Redundancy:** Keep names concise by avoiding repetitive terms.
- **Multiple Modifiers:** When multiple modifiers are required, arrange them logically and consistently.

By following these rules, we ensure that design tokens remain clear, scalable, and easy to maintain.

### Examples:
- `background-secondary-muted`
- `font-weight-bold`
- `button-border-hover`
  

## Design Token Usage

Not all design tokens will be necessary for every project, and you may need to introduce new ones. That's perfectly fine—just ensure that any additions adhere to the established naming conventions outlined above.

## Colors

### Primitive Colors

Primitive color tokens should correspond to either standard or brand colors. To enhance design flexibility, consider adding tints and shades, such as `color-primary-light`, `color-primary-dark`, and similar variants.

- `color-primary`
- `color-secondary`
- `color-accent`
- `color-muted`
- `color-inverse`
- `color-error`
- `color-warning`
- `color-danger`
- `color-success`
- `color-info`
- `color-disabled`

### Standard Colors

These colors are typically used in all projects and can be adjusted as needed.

- `color-black: 0 0% 3.9%`
- `color-white: 0 0% 98%`
- `color-gray-100: 0 0% 96.1%`
- `color-gray-200: 0 0% 89.8%`
- `color-gray-300: 0 0% 83.1%`
- `color-gray-400: 0 0% 63.9%`
- `color-gray-500: 0 0% 45.1%`
- `color-gray-600: 0 0% 32.2%`
- `color-gray-700: 0 0% 25.1%`
- `color-gray-800: 0 0% 14.9%`
- `color-gray-900: 0 0% 9%`

### Brand Colors

Brand specific color tints and shades.

- `color-red`
- `color-green`
- `color-blue`
- `color-yellow`
- ...

### Background

Pages, sections, elements and other background elements.

- `background`
- `background-muted`
- `background-inverse`
- `background-error`
- `background-warning`
- `background-danger`
- `background-success`
- `background-info`
- `background-disabled`
- `background-hover`
- `background-active`
- `background-secondary`
- `background-secondary-muted`
- `background-secondary-inverse`
- `background-secondary-error`
- `background-secondary-warning`
- `background-secondary-danger`
- `background-secondary-success`
- `background-secondary-info`
- `background-secondary-disabled`
- `background-secondary-hover`
- `background-secondary-active`
  
### Foreground

Text, borders, cards and other foreground elements.

- `foreground`
- `foreground-muted`
- `foreground-inverse`
- `foreground-error`
- `foreground-warning`
- `foreground-danger`
- `foreground-success`
- `foreground-info`
- `foreground-disabled`
- `foreground-hover`
- `foreground-active`
- `foreground-secondary`
- `foreground-secondary-muted`
- `foreground-secondary-inverse`
- `foreground-secondary-error`
- `foreground-secondary-warning`
- `foreground-secondary-danger`
- `foreground-secondary-success`
- `foreground-secondary-info`
- `foreground-secondary-disabled`
- `foreground-secondary-hover`
- `foreground-secondary-active`

### Link

- `link-color`
- `link-color-hover`
- `link-color-active`
- `link-color-visited`
- `link-color-muted`
- `link-color-hover-muted`
- `link-color-active-muted`
- `link-color-visited-muted`

### Button

- `button-background`
- `button-text`
- `button-border`
- `button-background-hover`
- `button-text-hover`
- `button-border-hover`
- `button-background-active`
- `button-text-active`
- `button-border-active`
- `button-background-visited`
- `button-text-visited`
- `button-border-visited`
- `button-background-muted`
- `button-text-muted`
- `button-border-muted`
- `button-background-muted-hover`
- `button-text-muted-hover`
- `button-border-muted-hover`
- `button-background-muted-active`
- `button-text-muted-active`
- `button-border-muted-active`
- `button-background-muted-visited`
- `button-text-muted-visited`
- `button-border-muted-visited`

### Border

- `border-color`
- `border-color-muted`
- `border-color-inverse`
- `border-color-error`
- `border-color-warning`
- `border-color-danger`
- `border-color-success`
- `border-color-info`
- `border-color-disabled`
- `border-color-hover`
- `border-color-active`

### Utility

- `focus-ring-color`
- `divider-color`

## Fonts

### Font Family

- `font-family-sans`
- `font-family-serif`

### Fonts

- `body-font`
- `body-font-muted`
- `headings-font`
- `headings-font-muted`

### Font Size

- `font-size-xs`
- `font-size-sm`
- `font-size-md` | `font-size-base`
- `font-size-lg`
- `font-size-xl`
- `font-size-2xl`
- `font-size-3xl`
- `font-size-4xl`
- `font-size-5xl`
- `font-size-6xl`

### Font Weight

- `font-weight-light: 300`
- `font-weight-normal: 400`
- `font-weight-medium: 500`
- `font-weight-bold: 700`
- `font-weight-extrabold: 800`
- `font-weight-black: 900`

### Line Height

- `line-height-none: 1`
- `line-height-tight: 1.25`
- `line-height-normal: 1.5`
- `line-height-relaxed: 1.75`
- `line-height-loose: 2`

### Letter Spacing

- `letter-spacing-tightest: -0.0625em`
- `letter-spacing-tighter: -0.03125em`
- `letter-spacing-tight: -0.015625em`
- `letter-spacing-normal: normal`
- `letter-spacing-wide: 0.03125em`
- `letter-spacing-wider: 0.0625em`
- `letter-spacing-widest: 0.09375em`

### Font Shorthand

Font shorthand is a way to define a font size, line height, and font weight using a single token. ([Reference](https://primer.style/foundations/primitives/typography#font-shorthand))

- `text-body-sm`
- `text-body-md` | `text-body`
- `text-body-lg`
- `text-title-sm`
- `text-title-md` | `text-title`
- `text-title-lg`
- `text-caption`
- `text-button-sm`
- `text-button-md` | `text-button`
- `text-button-lg`

## Spacing

- `space-xs`
- `space-sm`
- `space-md` | `space-base`
- `space-lg`
- `space-xl`
- `space-2xl`
- `space-3xl`
- `space-4xl`
- ...

## Sizing

### Max Width

- `max-width-none: none;`
- `max-width-auto: auto;`
- `max-width-full: 100%;`
- `max-width-container: 96rem;`
- `max-width-content: 40rem;`
- `max-width-breakout: 60rem;`

### Breakpoints

- `breakpoint-xs: 320px`
- `breakpoint-sm: 512px`
- `breakpoint-md: 768px`
- `breakpoint-lg: 1024px`
- `breakpoint-xl: 1280px`
- `breakpoint-2xl: 1536px`
- `breakpoint-3xl: 1782px`
- ...

## Animation

### Ease

- `ease-in: cubic-bezier(0.25, 0.0, 0.75, 0.25)`
- `ease-out: cubic-bezier(0.25, 0.75, 0.75, 1.0)`
- `ease-in-out: cubic-bezier(0.75, 0.25, 0.25, 0.75)`
- `ease-out-back: cubic-bezier(0.175, 0.885, 0.32, 1.275)`
- `ease-in-back: cubic-bezier(0.6, -0.28, 0.735, 0.045)`
- `ease-in-out-back: cubic-bezier(0.68, -0.55, 0.265, 1.55)`
- `ease-out-circ: cubic-bezier(0.075, 0.82, 0.165, 1.0)`
- `ease-in-circ: cubic-bezier(0.6, 0.04, 0.98, 0.335)`
- `ease-in-out-circ: cubic-bezier(0.785, 0.135, 0.15, 0.86)`

Easing reference ([Epiceasing.com](https://epiceasing.com/)).

### Duration

- `duration-immediate: 0s`
- `duration-faster: 0.15s`
- `duration-fast: 0.25s`
- `duration-slow: 0.35s`
- `duration-slower: 0.45s`

## Border

### Border Radius

- `border-radius-none: 0`
- `border-radius-base: 0.25rem`
- `border-radius-pill: 9999px`
- `border-radius-circle: 50%`
- ...

### Border width

- `border-width-none`
- `border-width-thin`
- `border-width-thick`
- ...

## Other Stuff

### Shadows

- `shadow-none`
- `shadow-elevation-1`
- `shadow-elevation-2`
- `shadow-elevation-3`
- `shadow-elevation-4`
- ...


## References

- [Token Naming Guidelines](https://nordhealth.design/naming/)
- [Token Naming Conventions](https://primer.style/foundations/primitives/token-names#convention-breakdown)
- [Naming Cheatsheet](https://github.com/kettanaito/naming-cheatsheet)
- [Naming Guide](https://classnames.paulrobertlloyd.com/)
- [Tokens, variables, and styles in Figma](https://help.figma.com/hc/en-us/articles/18490793776023-Update-1-Tokens-variables-and-styles)
- [Awesome Design Tokens](https://github.com/sturobson/Awesome-Design-Tokens?tab=readme-ov-file)
