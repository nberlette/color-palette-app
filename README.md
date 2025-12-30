<div align="center">

# 🎨 [colorspin](https://colorspin.vercel.app)

_Powerful interactive color palette generator app with tailwind and CSS export options._

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen?style=for-the-badge)](https://colorspin.vercel.app)
[![MIT License](https://img.shields.io/badge/license-MIT-blue?style=for-the-badge)](./LICENSE)
[![Built with Next.js](https://img.shields.io/badge/Next.js-15-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)

</div>

---

## Features

### Intelligent Color Generation

- **10-shade palettes** automatically generated from a single base color
- Smart lightness distribution from 50 (lightest) to 900 (darkest)
- Real-time preview as you adjust parameters

### Advanced Controls

- **Vibrancy slider**: Adjust color saturation intensity (0-100%)
- **Hue shift**: Rotate colors around the color wheel (-180° to +180°)
- **Interactive hex color picker** with live preview
- **Randomize button**: Generate inspiring color combinations instantly

### Multi-Palette Management

- Create and manage **multiple color sets** in one workspace
- Name each color set for easy organization
- Quick switching between palettes
- Delete individual sets (with safety guard for last palette)

### Color Harmony Explorer

Discover professional color schemes based on color theory:

- **Complementary**: Colors opposite on the wheel
- **Analogous**: Adjacent harmonious colors
- **Triadic**: Three evenly-spaced colors
- **Tetradic**: Four colors in complementary pairs
- **Split Complementary**: Base + two near-complement colors
- **Monochromatic**: Shades of a single hue

### Gradient Generator

- Create **linear** and **radial** gradients
- Add/remove color stops dynamically, adjust positions with sliders
- Control gradient angle (linear) or center (radial)

### Accessibility Tools

- **WCAG contrast ratio checker** for all shade combinations
- Automatic AA/AAA level compliance indicators
- Pass/fail status for text readability
- Ensures your designs are accessible to everyone

### Export Options

- **CSS custom properties** (CSS variables)
- **Tailwind config** (drop-in configuration)
- **JSON** (for programmatic use)
- **Gradient CSS** (ready-to-use code)

---

## Usage

### Creating Your First Palette

1. **Pick a base color** using the hex color picker or enter a hex value
2. **Adjust vibrancy** to control color saturation
3. **Apply hue shift** to explore color variations
4. **Click any shade** to copy its hex value to clipboard

### Exploring Color Harmonies

1. Navigate to the **"Harmonies"** tab
2. Browse color theory-based combinations
3. Click any harmony color to set it as your base color
4. Watch the palette regenerate instantly

### Building Gradients

1. Switch to the **"Gradients"** tab
2. Add color stops with the **"Add Stop"** button
3. Adjust stop positions and colors
4. Choose gradient type (linear/radial)
5. Set angle for linear gradients
6. Click **"Copy CSS"** to use in your project

### Checking Accessibility

1. Open the **"Contrast"** tab
2. Review contrast ratios for all shade pairs
3. Check WCAG AA/AAA compliance indicators
4. Ensure text meets accessibility standards

---

## Tech Stack

- **[Next.js 15](https://nextjs.org/)** - React framework with App Router
- **[React 19](https://react.dev/)** - JSX infrastructure
- **[TypeScript](https://www.typescriptlang.org/)** - Type safety
- **[Tailwind CSS](https://tailwindcss.com/)** - Utility-first styling
- **[Radix UI](https://www.radix-ui.com/)** - Accessible component primitives
- **[Framer Motion](https://www.framer.com/motion/)** - Smooth animations
- **[react-colorful](https://github.com/omgovich/react-colorful)** - Color picker
- **[next-themes](https://github.com/pacocoursey/next-themes)** - Dark mode support
- **[Lucide Icons](https://lucide.dev/)** - Beautiful icons

---

## Project Structure

```
colorspin/
├── app/                          # Next.js App Router
│   ├── layout.tsx               # Root layout with theme provider
│   ├── page.tsx                 # Home page
│   └── globals.css              # Global styles
├── components/
│   ├── color-palette-generator.tsx  # Main component (1600+ lines)
│   └── ui/                      # Shadcn/ui components
├── lib/
│   └── utils.ts                 # Utility functions
├── hooks/
│   └── use-toast.tsx            # Toast notification hook
├── styles/                       # Additional styles
├── public/                       # Static assets
└── tailwind.config.js           # Tailwind configuration
```

---

## 🎨 Color Science

ColorSpin uses **HSL (Hue, Saturation, Lightness)** color space for intelligent palette generation:

- **Hue** (0-360°): Position on the color wheel
- **Saturation** (0-100%): Color intensity/vibrancy
- **Lightness** (0-100%): Brightness of the color

This approach ensures:
- [x] Consistent lightness progression across shades
- [x] Natural-looking color variations
- [x] Better control over color relationships
- [x] Accessible contrast ratios

---

## Developing and Contributing

### Prerequisites

Since this project is built with [Next.js], it requires a Node-like[^1] runtime in order to
be deployed and function correctly. Additionally, some sort of package manager or dependency
management utility is required. I recommend using [Bun] or [Deno], since each of them serve
as both runtime **_and_** package manager, keeping things simple and centralized. They also
both support TypeScript and TSX as a first-class citizen with **zero extra configuration**.

### Installation

#### 1. Clone

##### `gh` ([GitHub CLI], recommended)

```bash
gh repo clone nberlette/colorspin
```

##### `git` (classic)

```bash
git clone https://github.com/nberlette/colorspin.git
```

###### First, change into the newly-cloned directory

```bash
cd colorspin
```

#### 2. Install

###### Bun

```bash
bun import && bun install # import from pnpm-lock.yaml or package-lock.json
```

###### Deno

```bash
deno install
```

###### PNPM

```bash
pnpm i
```

###### Yarn

```bash
yarn install
```

###### NPM

```bash
npm i
```

#### 3. Develop

```bash
bun dev
```

```bash
deno task dev
```

```bash
pnpm dev
```

```bash
yarn dev
```

```bash
npm run dev
```

> [!TIP]
>
> Open [http://localhost:3000](http://localhost:3000) to see the app in action! 🎉

---

## 🌟 Acknowledgments

- Inspired by tools like [Coolors](https://coolors.co/) and [Color Hunt](https://colorhunt.co/)
- Built with amazing open-source libraries
- Color theory principles from traditional design education

---

## 🔗 Links

- **Live Demo**: [colorspin.vercel.app](https://colorspin.vercel.app)
- **Repository**: [github.com/nberlette/colorspin](https://github.com/nberlette/colorspin)
- **Issues**: [Report a bug or request a feature](https://github.com/nberlette/colorspin/issues)

---

<div align="center">

**Made with ❤️ by [Nicholas Berlette](https://github.com/nberlette)**. [MIT License].

<small>
  
_If you find this useful, please consider giving it a ⭐️!_

</small></div>

[Next.js]: https://nextjs.org
[GitHub CLI]: https://cli.github.com
[MIT License]: https://nick.mit-license.org/2024
[Nicholas Berlette]: https://github.com/nberlette
[GitHub]: https://github.com/nberlette/colorspin/#readme
[issues]: https://github.com/nberlette/colorspin/issues
[vercel]: https://vercel.com
[colorspin]: https://colorspin.vercel.app
