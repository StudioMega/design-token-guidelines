# Mega Design Token Guidelines

Design tokens are standardized, reusable variables that store design decisions, such as colors, fonts, spacing, and other visual elements. These tokens help maintain consistency across a product or design system by ensuring that these elements are applied uniformly across different platforms and devices.

## Table Of Contents

- [Why Use Design Tokens?](#why-use-design-tokens)
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

## Colors

### Primitives

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

### Brand Primitives

- `color-red`
- `color-green`
- `color-blue`
- `color-yellow`
- ...

### Background

- `color-background-primary`
- `color-background-muted`
- `color-background-error`
- `color-background-warning`
- `color-background-danger`
- `color-background-success`
- `color-background-info`
- `color-background-disabled`

  
### Foreground (text)

- `color-foreground-primary`
- `color-foreground-muted`
- `color-foreground-error`
- `color-foreground-warning`
- `color-foreground-danger`
- `color-foreground-success`
- `color-foreground-info`
- `color-foreground-disabled`

### Link

- `color-link-primary`
- `color-link-primary-hover`
- `color-link-primary-active`
- `color-link-primary-visited`
- `color-link-muted`
- `color-link-muted-hover`
- `color-link-muted-active`
- `color-link-muted-visited`

### Button

- `color-button-primary`
- `color-button-primary-hover`
- `color-button-primary-active`
- `color-button-primary-visited`
- `color-button-muted`
- `color-button-muted-hover`
- `color-button-muted-active`
- `color-button-muted-visited`

### Border

- `color-border-primary`
- `color-border-muted`

### Utility

- `color-focus-ring`
- `color-divider`

## Fonts

### Font Family

- `font-family-sans`
- `font-family-serif`
- `font-family-body`
- `font-family-body-muted`
- `font-family-headings`
- `font-family-headings-muted`

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
- `shadow-sm`
- `shadow-md`
- `shadow-lg`
- `shadow-xl`
- `shadow-2xl`
- ...

## Notes
- Possible color naming could be "weaker" to "stronger" https://protocol.mozilla.org/docs/fundamentals/color
- Naming opposites "primary" to "inverse"

## References

- [Token Naming Guidelines](https://nordhealth.design/naming/)
- [Token Naming Conventions](https://primer.style/foundations/primitives/token-names#convention-breakdown)
- [Naming Cheatsheet](https://github.com/kettanaito/naming-cheatsheet)
- [Naming Guide](https://classnames.paulrobertlloyd.com/)
- [Tokens, variables, and styles in Figma](https://help.figma.com/hc/en-us/articles/18490793776023-Update-1-Tokens-variables-and-styles)
- [Awesome Design Tokens](https://github.com/sturobson/Awesome-Design-Tokens?tab=readme-ov-file)
