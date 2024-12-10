![NSG CSS Utilities](https://i.ibb.co/ZJJMgPS/nsg-utils.jpg)

# NOSTO GLOBAL CSS Utilities

A comprehensive CSS utility library for rapid web development, built using Atomic CSS methodology and inspired by SCSS @extend patterns.

## Features

- Typography utilities with scalable font sizes
- Flexible spacing system with margin and padding utilities
- Display and positioning helpers
- Flexbox and Grid utilities
- Dimension controls
- Reset utilities
- Border and visibility helpers
- Easy responsiveness through REM units and consistent scaling

## Architecture

- Follows CSS Bricks methodology for small, reusable utility classes
- Inspired by SCSS @extend patterns for clean CSS organization
- Uses REM units with consistent scale factor for responsive design
  - All measurements scale proportionally with root font size
  - Makes responsive design more manageable

## Core Variables

The library uses CSS custom properties for consistent theming:

```css
--nsg-base-size: 1rem
--nsg-scale: 1.25
--nsg-gap: 1rem
```

These variables ensure consistent scaling across your application, making it easier to maintain responsive designs by simply adjusting the root font size.

## Usage Examples

### Custom CSS Default Variables

For example The default gap value of 1rem can be overridden using CSS custom properties. Set the --nsg-gap variable directly in the style attribute when you need custom spacing between flex or grid items

```html
<div
  class="nsg-d-flex"
  style="--nsg-gap: 2rem;"
>
  Elements with 2rem gap between them
</div>
```

### Typography

```html
<div class="nsg-fs-3 nsg-fw-4">
  Bold, larger text with font-size level 3 and font-weight level 4
</div>
```

### Spacing

```html
<div class="nsg-m-3 nsg-p-2">
  Element with margin level 3 and padding level 2
</div>
```

### Flexbox

```html
<div class="nsg-d-flex nsg-justify-center nsg-align-center">
  Centered flex container with justify-content: center and align-items: center
</div>
```

### Positioning

```html
<div class="nsg-relative">
  <div class="nsg-absolute">
    Absolutely positioned element inside a relative container
  </div>
</div>
```

## Available Classes

- Font sizes: `nsg-fs-1` through `nsg-fs-5`
- Font weights: `nsg-fw-1` through `nsg-fw-5`
- Margins/Padding: `nsg-m-0` through `nsg-m-5`, `nsg-p-0` through `nsg-p-5`
- Display: `nsg-d-block`, `nsg-d-flex`, `nsg-d-grid`, etc.
- Position: `nsg-relative`, `nsg-absolute`, `nsg-fixed`, `nsg-sticky`
- And many more...

## Resources

### Atomic CSS

- [Atomic CSS ](https://compiledcssinjs.com/docs/atomic-css)

### SCSS @extend Pattern Resources

- [Sass @extend ](https://sass-lang.com/guide/#mixins)

## Upcoming Features

The following features are planned for future releases:

### Grid System

- Complete grid layout utilities
- Grid flow controls

### Animation System

- Transition utilities
- Animation classes
- Timing and delay controls

These features are currently in development and will be added in upcoming versions.

### Credit

- [Cover Image - Rachel by Jan De Coster](https://www.behance.net/gallery/17061285/Rachel-Melting-Robot-Hearts)
- [Talk about Rachel and more by Jan De Coster at Beyond Tellernad 2024](https://youtu.be/XxDnTDe36Oc?si=je7m93kfGUiSPq6t)
