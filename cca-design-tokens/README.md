# CCA Design Tokens

Design tokens for Token Studio (Figma). This folder contains all tokens synced with Token Studio.

## Files

- **`tokens.json`** - Main Token Studio file with all color and existing tokens
- **`typography-primitives.json`** - Base typography values (font families, weights, sizes for Desktop/Mobile)
- **`typography-system.json`** - Semantic typography tokens (heading, body, label, code, link, input)

## Typography System (UI Prep Structure)

### Typography Primitives

**Font Families:**
- Sans: Helvetica Neue, Helvetica, Arial, sans-serif
- Mono: ui-monospace, system monospace

**Font Weights:**
- Regular: 400
- Semibold: 600
- Bold: 700
- Italic: italic

**Font Size Scale (with Desktop & Mobile modes):**
- Desktop: 50 (11px) → 1300 (60px)
- Mobile: 50 (13px) → 1300 (70px)

### Typography System (Semantic Tokens)

All semantic tokens reference the primitives and support Desktop/Mobile modes:

- **Heading**: Sans family, Bold weight, Sizes XL/L/M/S
- **Body**: Sans/Mono family, Regular/Semibold/Italic weight, Sizes L/M/S/XS  
- **Label**: Sans family, Semibold weight, Sizes L/M/S/XS
- **Code**: Mono family, Regular weight, Sizes L/M/S
- **Link**: Sans family, Semibold weight, Sizes L/M/S/XS
- **Input**: Sans family, Regular weight, Sizes L/M/S

## Using in Token Studio

1. Open Token Studio plugin in Figma
2. Go to Settings → Storage → Pull from GitHub
3. Token Studio will load all three JSON files
4. Set up Desktop/Mobile modes for responsive typography

## Using in Code

After pulling these tokens into your project and building:

```tsx
// Heading XL with Desktop/Mobile responsive sizes
<h1 className="text-heading-size-xl-desktop md:text-heading-size-xl-mobile font-bold">

// Body M with strong weight
<p className="text-body-size-m-desktop md:text-body-size-m-mobile font-semibold">

// Label S
<span className="text-label-size-s-desktop md:text-label-size-s-mobile">
```
