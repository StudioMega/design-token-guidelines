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

Not all design tokens will be necessary for every project, and you may need to introduce new ones. That's perfectly fine—just ensure that any additions adhere to the [established naming conventions](#design-token-naming).

## Colors

### Primitive Colors

Primitive color tokens should correspond to either standard or brand colors. To enhance design flexibility, consider adding tints and shades, such as `color-primary-light`, `color-primary-dark`, and similar variants. Use [HSL](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value/hsl) color values for these tokens.

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

CSS Example: `--color-primary: hsl(46, 100%, 50%);`

### Standard Colors

These colors are typically used in all projects and can be adjusted as needed. Use [HSL](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value/hsl) color values for these tokens.

- `color-black`
- `color-white`
- `color-gray-100`
- `color-gray-200`
- `color-gray-300`
- `color-gray-400`
- `color-gray-500`
- `color-gray-600`
- `color-gray-700`
- `color-gray-800`
- `color-gray-900`

CSS Example: `--color-black: hsl(0, 0%, 0%);`

### Brand Colors

Brand specific color tints and shades. Use [HSL](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value/hsl) color values for these tokens.

- `color-red`
- `color-green`
- `color-blue`
- `color-yellow`
- ...

CSS Example: `--color-yellow: hsl(60, 100%, 50%);`

### Background

Pages, sections, elements and other background elements. Use [HSL](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value/hsl) color values for these tokens when not referencing another color token.

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
  
CSS Example: `--background: var(--color-black);`

### Foreground

Text, borders, cards and other foreground elements. Use [HSL](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value/hsl) color values for these tokens when not referencing another color token.

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

CSS Example: `--foreground: var(--color-white);`

### Link

- `link-color`
- `link-color-hover`
- `link-color-active`
- `link-color-visited`
- `link-color-muted`
- `link-color-hover-muted`
- `link-color-active-muted`
- `link-color-visited-muted`

CSS Example: `--link-color: var(--color-blue);`

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

CSS Example: `--button-background: var(--color-blue);`

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

CSS Example: `--border-color: var(--color-black);`

### Utility

- `focus-ring-color`
- `divider-color`

CSS Example: `--focus-ring-color: var(--color-blue);`

## Fonts

### Font Family

These are the font families that are available to use. The values should be the font family names.

- `font-family-sans`
- `font-family-serif`

### Fonts

- `body-font`
- `body-font-muted`
- `headings-font`
- `headings-font-muted`

CSS Example: `--body-font: var(--font-family-sans);`

### Font Size

All fonts larger than 24px should be calculated using [clamp()](https://utopia.fyi/clamp/calculator?a=320,1240) to ensure that they are responsive.

Font sizes are using default values.
  
- `--font-size--2: 0.75rem;` _12px_
- `--font-size--1: 0.875rem;` _14px_
- `--font-size-0: 1rem;` _16px_
- `--font-size-1: 1.125rem;` _18px_
- `--font-size-2: 1.25rem;` _20px_
- `--font-size-3: 1.5rem;` _24px_
- `--font-size-4: clamp(1.5rem, 1.375rem + 0.625vw, 1.875rem);` _24px > 30px_
- `--font-size-5: clamp(1.875rem, 1.75rem + 0.625vw, 2.25rem);` _30px > 36px_
- `--font-size-6: clamp(2.25rem, 2rem + 1.25vw, 3rem);` _36px > 48px_
- `--font-size-7: clamp(3rem, 2.75rem + 1.25vw, 3.75rem);` _48px > 60px_
- `--font-size-8: clamp(3.75rem, 3.5rem + 1.25vw, 4.5rem);` _60px > 72px_

### Font Weight

Font weights are using default values.

- `--font-weight-light: 300;  `
- `--font-weight-normal: 400;`
- `--font-weight-medium: 500;`
- `--font-weight-bold: 700;`
- `--font-weight-extrabold: 800;`
- `--font-weight-black: 900;`

### Line Height

Line heights are using default values.

- `--line-height-none: 1;`
- `--line-height-tight: 1.15;`
- `--line-height-snug: 1.375;`
- `--line-height-normal: 1.5;`
- `--line-height-relaxed: 1.75;`
- `--line-height-loose: 2;`

### Letter Spacing

Letter spacing is using default values.

- `--letter-spacing-tightest: -0.0625em;`
- `--letter-spacing-tighter: -0.03125em;`
- `--letter-spacing-tight: -0.015625em;`
- `--letter-spacing-normal: normal;`
- `--letter-spacing-wide: 0.02125em;`
- `--letter-spacing-wider: 0.0625em;`
- `--letter-spacing-widest: 0.09375em;`

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

All spacing larger than 24px should be calculated using [clamp()](https://utopia.fyi/clamp/calculator?a=320,1240) to ensure that they are responsive. 

Spacing values are using default values.

- `--space-2xs: 0.25rem;` _4px_
- `--space-xs: 0.5rem;` _8px_
- `--space-s: 0.75rem;` _12px_
- `--space-m: 1rem;` _16px_
- `--space-l: 1.5rem;` _24px_
- `--space-xl: clamp(2rem, 1.6667rem + 1.6667vw, 3rem);` _32px > 48px_
- `--space-2xl: clamp(3rem, 2rem + 5vw, 6rem);` _48px > 96px_
- `--space-3xl: clamp(6rem, 5.3333rem + 3.3333vw, 8rem);` _96px > 128px_
- `--space-4xl: clamp(8rem, 6.6667rem + 6.6667vw, 12rem);` _128px > 192px_
- `--space-5xl: clamp(12rem, 10.6667rem + 6.6667vw, 16rem);` _192px > 256px_

## Sizing

### Max Width

Max width values are using default values.

- `--max-width-none: none;`
- `--max-width-auto: auto;`
- `--max-width-full: 100%;`
- `--max-width-container: 96rem;`
- `--max-width-content: 40rem;`
- `--max-width-breakout: 60rem;`

### Breakpoints

Breakpoints are using default values.

- `--breakpoint-xs: 320px;`
- `--breakpoint-sm: 512px;`
- `--breakpoint-md: 768px;`
- `--breakpoint-lg: 1024px;`
- `--breakpoint-xl: 1280px;`
- `--breakpoint-2xl: 1536px;`
- `--breakpoint-3xl: 1782px;`
- ...

## Animation

### Ease

Ease values are using default values.

- `--ease-in: cubic-bezier(0.25, 0, 0.75, 0.25);`
- `--ease-out: cubic-bezier(0.25, 0.75, 0.75, 1);`
- `--ease-in-out: cubic-bezier(0.75, 0.25, 0.25, 0.75);`
- `--ease-out-back: cubic-bezier(0.175, 0.885, 0.32, 1.275);`
- `--ease-in-back: cubic-bezier(0.6, -0.28, 0.735, 0.045);`
- `--ease-in-out-back: cubic-bezier(0.68, -0.55, 0.265, 1.55);`
- `--ease-out-circ: cubic-bezier(0.075, 0.82, 0.165, 1);`
- `--ease-in-circ: cubic-bezier(0.6, 0.04, 0.98, 0.335);`
- `--ease-in-out-circ: cubic-bezier(0.785, 0.135, 0.15, 0.86);`
- `--ease-in-quint: cubic-bezier(0.755, 0.05, 0.855, 0.06);`
- `--ease-out-quint: cubic-bezier(0.23, 1, 0.32, 1);`
- `--ease-in-out-quint: cubic-bezier(0.87, 0, 0.13, 1);`

Easing reference ([Epiceasing.com](https://epiceasing.com/)).

### Duration

Duration values are using default values.

- `--duration-immediate: 0s;`
- `--duration-faster: 0.15s;`
- `--duration-fast: 0.25s;`
- `--duration-slow: 0.35s;`
- `--duration-slower: 0.45s;`
- `--duration-slowest: 0.65s;`

## Border

### Border Radius

Border radius values are using default values.

- `--border-radius-none: 0;`
- `--border-radius-base: 0.25rem;`
- `--border-radius-pill: 9999px;`
- `--border-radius-circle: 50%;`
- ...

### Border width

Border width values are using default values.

- `--border-width-none: 0px;`
- `--border-width-thin: 1px;`
- `--border-width-thick: 2px;`
- ...

## Other Stuff

### Shadows

Shadows are using default values.

- `--shadow-none: box-shadow: 0 0 #0000;`
- `--shadow-elevation-1:box-shadow: 0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);`
- `--shadow-elevation-2: box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);`
- `--shadow-elevation-3: box-shadow: 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);`
- `--shadow-elevation-4: 	box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);`
- ...


## References

- [Token Naming Guidelines](https://nordhealth.design/naming/)
- [Token Naming Conventions](https://primer.style/foundations/primitives/token-names#convention-breakdown)
- [Naming Cheatsheet](https://github.com/kettanaito/naming-cheatsheet)
- [Naming Guide](https://classnames.paulrobertlloyd.com/)
- [Tokens, variables, and styles in Figma](https://help.figma.com/hc/en-us/articles/18490793776023-Update-1-Tokens-variables-and-styles)
- [Awesome Design Tokens](https://github.com/sturobson/Awesome-Design-Tokens?tab=readme-ov-file)
