# FabrikFit - Ecommerce Frontend (React + Vite + Tailwind CSS)

FabrikFit is a modern, responsive ecommerce frontend built with React, Vite, and Tailwind CSS. It showcases a fashion storefront with a hero section, product filtering UI, product grid with load-more behavior, collection highlights, and a slide-in shopping cart drawer.

## Tech Stack
- **Frontend**: React 19, React DOM 19
- **Build Tool**: Vite 7
- **Styling**: Tailwind CSS 4 (via `@tailwindcss/vite`)
- **Icons**: `react-icons`
- **Linting**: ESLint 9 with React Hooks and React Refresh plugins

## Features
- **Responsive layout**: Mobile-first navigation with hamburger menu and dropdowns
- **Hero section**: Large banner with call-to-action buttons
- **Filter bar**: Select inputs for price, product type, brand, availability, color, and size (UI only)
- **Product grid**: 12 demo products with sale badges, sold-out states, hover effects, and a manual "Load More" interaction
- **Collections slider/cards**: Highlighted collection cards with images and CTA buttons
- **Shopping cart drawer**: Slide-in cart panel with click-outside-to-close behavior (demo state)
- **Footer**: Multi-column footer with collapsible sections on mobile and social/payment icons

## Getting Started

### Prerequisites
- Node.js 18+ and npm

### Installation
```bash
npm install
```

### Development
Run the dev server with hot module replacement:
```bash
npm run dev
```
The app will start and Vite will print a local URL (typically `http://localhost:5173`).

### Build
Create a production build:
```bash
npm run build
```
Preview the built app locally:
```bash
npm run preview
```

## Project Structure
```
├─ index.html
├─ package.json
├─ vite.config.js
├─ src/
│  ├─ main.jsx            # React entry (StrictMode)
│  ├─ App.jsx             # Page composition
│  ├─ index.css           # Tailwind CSS entry (@import "tailwindcss")
│  ├─ assets/             # Images (hero, collections, products)
│  └─ components/
│     ├─ Header.jsx       # Responsive header, menus, cart trigger
│     ├─ Hero.jsx         # Hero banner
│     ├─ FilterBar.jsx    # Filter selects (UI only)
│     ├─ ProductGrid.jsx  # Demo products + Load More
│     ├─ CollectionSlider.jsx # Collection highlight cards
│     ├─ ShoppingCart.jsx # Slide-in drawer
│     └─ Footer.jsx       # Footer with newsletter & icons
```

## Customization
- Update images in `src/assets/` to match your brand.
- Edit navigation items and dropdowns in `src/components/Header.jsx`.
- Adjust demo product data in `src/components/ProductGrid.jsx`.
- Tweak Tailwind classes across components for colors, spacing, and typography.

## Notes
- Filters and cart are UI demos only—no backend or stateful cart logic is implemented.
- Tailwind CSS v4 is configured via the Vite plugin `@tailwindcss/vite`. No separate Tailwind config file is present.

## Scripts
- **dev**: start Vite dev server
- **build**: production build
- **preview**: preview production build
- **lint**: run ESLint on the project

## License
This project is for educational/demo purposes. Add your preferred license if you plan to distribute.
