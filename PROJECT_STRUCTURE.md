# Cleric - Project Structure

This document outlines the comprehensive project structure implemented for the Cleric AstroJS website.

## 📁 Project Overview

```
curved-corot/
├── src/
│   ├── assets/                 # Static assets
│   │   ├── images/            # Image files
│   │   ├── icons/             # Icon files
│   │   ├── fonts/             # Custom fonts
│   │   └── videos/            # Video files
│   ├── components/            # Reusable components
│   │   ├── ui/               # Basic UI components (buttons, inputs, etc.)
│   │   ├── layout/           # Layout-specific components
│   │   ├── sections/         # Page section components
│   │   ├── forms/            # Form components
│   │   ├── navigation/       # Navigation components
│   │   └── media/            # Media-related components
│   ├── layouts/              # Page layout templates
│   │   ├── partials/         # Partial layout components
│   │   └── templates/        # Full page templates
│   ├── pages/                # Route pages
│   │   ├── api/              # API endpoints
│   │   ├── blog/             # Blog pages
│   │   └── products/         # Product pages
│   ├── styles/               # CSS and styling
│   │   ├── base/             # Base styles, variables, typography
│   │   ├── components/       # Component-specific styles
│   │   ├── layouts/          # Layout-specific styles
│   │   ├── utilities/        # Utility classes and helpers
│   │   └── themes/           # Theme variations
│   ├── lib/                  # Utility libraries and helpers
│   │   ├── utils/            # Utility functions
│   │   ├── constants/        # Application constants
│   │   ├── api/              # API utilities
│   │   └── validation/       # Validation helpers
│   ├── types/                # TypeScript type definitions
│   ├── hooks/                # Custom hooks (if using React/Vue components)
│   └── data/                 # Static data files
├── public/                   # Public static files
├── .vscode/                  # VSCode configuration
├── package.json              # Dependencies and scripts
├── package-lock.json         # Dependency lock file
├── astro.config.mjs          # Astro configuration
├── tsconfig.json             # TypeScript configuration
└── README.md                 # Project documentation
```

## 🎨 Design System

### CSS Architecture

**Base Layer** (`src/styles/base/`):
- `variables.css` - CSS custom properties for colors, typography, spacing
- `reset.css` - Modern CSS reset
- `typography.css` - Typography styles and utilities

**Utilities Layer** (`src/styles/utilities/`):
- `responsive.css` - Responsive utilities and grid system

**Components Layer** (`src/styles/components/`):
- Component-specific styling

### Color System

```css
/* Primary Brand Colors */
--color-cleric-primary: #4361EE
--color-cleric-blue: #4361EE
--color-cleric-blue-dark: #3046D1
--color-cleric-blue-light: #5B73F0

/* Hero Section */
--color-hero-bg: linear-gradient(135deg, #4361EE 0%, #7209b7 35%, #f72585 100%)
--color-hero-text: #ffffff
--color-hero-text-secondary: rgba(255, 255, 255, 0.9)
```

### Typography

```css
/* Font Families */
--font-family-primary: 'Inter', sans-serif

/* Fluid Typography */
--font-size-hero-title: clamp(2.5rem, 5vw, 4.5rem)
--font-size-hero-subtitle: clamp(1.125rem, 2.5vw, 1.5rem)
```

## 🧩 Component Architecture

### Navigation Components

**Header** (`src/components/navigation/Header.astro`):
- Responsive navigation with mobile menu
- Logo and brand positioning
- CTA button integration
- Dropdown menu support

### Section Components

**Hero** (`src/components/sections/Hero.astro`):
- Full-screen hero section with gradient background
- Press release badge component
- Dual CTA buttons (primary/secondary)
- Product interface mockup placeholder
- Responsive grid layout

### Layout Components

**Layout** (`src/layouts/Layout.astro`):
- Base HTML structure
- Meta tags and SEO optimization
- Global styles import
- Font loading optimization

## 📱 Responsive Design

### Breakpoint System

```css
--breakpoint-sm: 640px   /* Mobile landscape */
--breakpoint-md: 768px   /* Tablet */
--breakpoint-lg: 1024px  /* Desktop */
--breakpoint-xl: 1280px  /* Large desktop */
```

### Responsive Strategy

- **Mobile-first approach** with progressive enhancement
- **Fluid typography** using clamp() for optimal scaling
- **Flexible grid system** with CSS Grid and Flexbox
- **Component-level responsive behavior**

### Key Responsive Features

- Navigation transforms to mobile menu on smaller screens
- Hero section stacks vertically on tablets and mobile
- Interface mockup adapts to container size
- Typography scales fluidly across all devices

## 🛠️ Development Tools

### TypeScript Integration

**Type Definitions** (`src/types/index.ts`):
- Component prop interfaces
- Global utility types
- API response types
- Theme configuration types

**Utility Functions** (`src/lib/utils/index.ts`):
- Helper functions for common operations
- Responsive utility functions
- Validation helpers
- Date/time formatting

### Constants Management

**Application Constants** (`src/lib/constants/index.ts`):
- Site configuration
- API endpoints
- Validation patterns
- Feature flags

## 🎯 Key Features Implemented

### ✅ Complete Hero Section
- [x] Responsive navigation header
- [x] Gradient background with brand colors
- [x] Typography hierarchy with proper scaling
- [x] Dual CTA button system
- [x] Product interface mockup placeholder
- [x] Press release notification badge

### ✅ Responsive Design System
- [x] Mobile-first CSS architecture
- [x] Fluid typography system
- [x] Flexible component layouts
- [x] Cross-device compatibility

### ✅ Development Infrastructure
- [x] TypeScript type definitions
- [x] Utility function library
- [x] CSS custom properties system
- [x] Component organization structure

## 🚀 Getting Started

1. **Install Dependencies**:
   ```bash
   npm install
   ```

2. **Start Development Server**:
   ```bash
   npm run dev
   ```

3. **Build for Production**:
   ```bash
   npm run build
   ```

## 📝 Next Steps

The foundation is now ready for:

1. **Content Integration**: Replace placeholders with actual Figma designs
2. **Additional Sections**: Build out remaining page sections
3. **Interactive Elements**: Add animations and micro-interactions
4. **CMS Integration**: Connect with content management system
5. **Performance Optimization**: Implement image optimization and lazy loading

## 🎨 Design Implementation Notes

The current hero section matches the provided screenshot with:
- Accurate color scheme and gradients
- Proper typography hierarchy
- Responsive button styling
- Interface mockup placeholder structure
- Cross-device layout adaptation

All styling uses CSS custom properties for easy theming and maintenance, and the component structure supports easy expansion and modification.