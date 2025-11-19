# Foodies Organic Food Store - Complete Design Guide

## Table of Contents
1. [Design System Overview](#design-system-overview)
2. [Color Palette](#color-palette)
3. [Typography](#typography)
4. [Layout & Spacing](#layout--spacing)
5. [Component Library](#component-library)
6. [Section Specifications](#section-specifications)
7. [Responsive Behavior](#responsive-behavior)
8. [Implementation Guidelines](#implementation-guidelines)

---

## Design System Overview

Foodies is an organic food store website built with a modern, clean design system focused on accessibility, usability, and visual consistency. The design uses Inter as the primary typeface with a green color scheme that reflects the organic and natural brand identity.

---

## Color Palette

### Primary Colors
| Color | HEX | Usage |
|-------|-----|-------|
| Primary Green | `#06C167` | Buttons, icons, highlights, active states |
| Light Background | `#F3FAFB` | Card backgrounds, image containers |
| Input Background | `#F0F1EC` | Form inputs, search fields |
| White | `#FFFFFF` | Backgrounds, text on colored backgrounds |

### Text Colors
| Color | HEX | Usage |
|-------|-----|-------|
| Dark Text | `#1D1D1F` | Headings, primary text |
| Secondary Text | `#394149` | Body text, descriptions |
| Border Color | `#76767540` (25% opacity) | Card borders, dividers |

### Functional Colors
| Element | Color | Usage |
|---------|-------|-------|
| Success | `#06C167` | Positive actions, ratings |
| Error | `#DC3545` | Error states, warnings |
| Warning | `#FFC107` | Notifications, alerts |

---

## Typography

### Font Family
- **Primary**: Inter
- **Fallback Stack**: `Inter, system-ui, -apple-system, sans-serif`

### Scale & Hierarchy

| Element | Size | Weight | Line Height | Use Case |
|---------|------|--------|-------------|----------|
| Hero/Headline Large | 60px | 500 (Medium) / 600 (Semi Bold) | 100% | Hero sections, major headings |
| Section Headers | 60px | 500 (Medium) | 100% | Benefits, Our Stars, Features |
| Card Headers | 32px | 500 (Medium) | 100% | Feature cards, product titles |
| Stats Display | 40px | 600 (Semi Bold) | 100% | Statistics in Our Stars section |
| Footer Headers | 24px | 500 (Medium) | 100% | Footer section headings |
| Body Large | 16px | 400 (Regular) | 160% | Paragraphs, navigation, product info |
| Body Small | 15px | 400 (Regular) / 500 (Medium) | 100% | Small text, benefits p-tags |
| Button Text | 15px-16px | 400-500 (Regular-Medium) | 100% | All button elements |
| Label Text | 14px | 500 (Medium) | 100% | Form labels, captions |

### Typography Rules
- **Letter Spacing**: 0% (default)
- **Text Transform**: None (use proper casing)
- **Text Decoration**: Underline only for links on hover

---

## Layout & Spacing

### Grid System
```css
/* Desktop (1200px+) */
Grid: 12-column
Gutter: 30px
Margin: 132px (sides)

/* Tablet (768px - 1199px) */
Grid: 8-column  
Gutter: 24px
Margin: 60px (sides)

/* Mobile (320px - 767px) */
Grid: 4-column
Gutter: 20px
Margin: 20px (sides)
```

### Spacing Scale
| Token | Value | Use Case |
|-------|-------|----------|
| Space-xs | 8px | Icon padding, small gaps |
| Space-sm | 16px | Button padding, card padding |
| Space-md | 24px | Section padding, image padding |
| Space-lg | 32px | Between major sections |
| Space-xl | 40px | Large gaps, between components |
| Space-xxl | 60px-80px | Between page sections |

### Border Radius
| Token | Value | Use Case |
|-------|-------|----------|
| Radius-sm | 12px | Buttons, small cards, images |
| Radius-md | 16px | Banners, medium containers |
| Radius-lg | 24px | Large image containers, feature blocks |

---

## Component Library

### Buttons

#### Primary Button
```css
/* Layout */
Width: 200px
Height: 67.9px
Border Radius: 12px

/* Colors */
Background: #06C167
Text: #FFFFFF

/* Typography */
Font: Inter, 500, 16px
Line Height: 100%
Letter Spacing: 0%

/* States */
Hover: transform: translateY(-2px), box-shadow
Active: scale(0.98)
Disabled: opacity: 0.6
```

#### Secondary Button
```css
/* Layout */
Padding: 12px 24px
Border Radius: 12px

/* Colors */
Background: Transparent
Border: 1px solid #06C167
Text: #06C167

/* Typography */
Font: Inter, 500, 15px
Line Height: 100%

/* States */
Hover: Background: #06C167, Text: #FFFFFF
```

#### CTA Button
```css
/* Layout */
Width: 148px
Height: 41.94px

/* Colors */
Background: #06C167
Text: #FFFFFF

/* Typography */
Font: Inter, 500, 15px
Line Height: 100%
```

#### Subscribe Button
```css
/* Layout */
Width: 118px
Height: 49.93px
Border Radius: 12px

/* Colors */
Background: #06C167
Text: #FFFFFF
```

### Form Elements

#### Input Field
```css
/* Layout */
Width: 205px
Height: 49.93px
Border Radius: 12px
Padding: 12px 16px

/* Colors */
Background: #F0F1EC
Border: 1px solid transparent
Text: #1D1D1F

/* States */
Focus: border-color: #06C167
Error: border-color: #DC3545
```

### Cards

#### Product Card
```css
/* Layout */
Width: 270px
Height: 444px
Border Radius: 12px
Border: 2px solid #76767540

/* Special State */
First Card: border: 1px solid #06C167

/* Content */
Image: Full width, aspect ratio 4:3
Text: Left aligned
Rating: #06C167 stars
```

#### Feature Card
```css
/* Layout */
Width: 292.5px
Height: 292.08px
Background: #F3FAFB
Border Radius: 12px
Padding: 30px

/* Content */
Text: Centered vertically
CTA: Bottom aligned
```

### Navigation

#### Desktop Navigation
```css
/* Layout */
Margin Top: 42px
Item Spacing: 30px

/* Typography */
Font: Inter, 500, 16px
Text: #FFFFFF

/* States */
Hover: opacity: 0.8
Active: color: rgba(255,255,255,0.9)
```

#### Mobile Navigation
```css
/* Toggle Button */
Width: 30px
Height: 21px
Color: #FFFFFF

/* Menu Panel */
Background: #06C167
Position: Fixed top
Animation: Slide down
```

---

## Section Specifications

### Header & Hero Section
```css
/* Background */
Background: #06C167

/* Hero Layout */
Text: Left 50%, Image: Right 50%
Hero Image: 468px × 515.26px, radius: 12px

/* Content */
Headline: 60px, #FFFFFF
Description: 16px, rgba(255,255,255,0.9)
```

### Brands Section
```css
/* Container */
Width: 1194.89px
Height: 49px
Gap: 40px
Background: #394149
Opacity: 55%

/* Logo Behavior */
Hover: opacity: 1
Mobile: 2 logos per row
```

### Highlights Features
```css
/* Container */
Width: 1170px
Height: 184.73px

/* Item Layout */
Image: Left aligned
Content: Right aligned, 2 lines
Spacing: 20px between image and text
```

### Benefits Section
```css
/* Layout */
Image: Left, Content: Right
Image Container: 493px × 560.26px, radius: 24px
Inner Image: 445px × 512.26px, radius: 12px
Background: #F3FAFB
Padding: 24px

/* Icons */
Size: 26px × 19.36px
Color: #06C167
```

### Our Stars Section
```css
/* Layout */
Content: Left, Image: Right
Image Container: 541px × 607.13px
Background: #F3FAFB
Inner Image: 445px × 512.26px

/* Stats */
Number: 40px, Semi Bold, #06C167
Label: 15px, Regular, #1D1D1F
```

### Features Section
```css
/* Header */
P Tag Container: 175px × 48px, radius: 12px
Background: #F3FAFB
Border: 1px solid #06C167
Padding: 12px 24px
Alignment: Centered

/* Grid */
Desktop: 4 columns × 2 rows
Mobile: 2 columns × 4 rows
Card Size: 292.5px × 292.08px
```

### Our Products Section
```css
/* Layout */
Text Alignment: Top left
Grid: 4 columns desktop, 2 mobile, 1 small mobile

/* Color Accents */
Star Icons: #06C167
Discounted Price: #06C167  
Button Text: #06C167
```

### Pre-footer Banner
```css
/* Container */
Width: 1170px
Height: 458.34px
Border Radius: 16px
Full Width Section

/* Content */
Background Image with overlay
Text: Centered
Headline: 60px, Semi Bold, #FFFFFF
```

### Footer Section
```css
/* Layout */
Grid: 4 columns desktop, 2 tablet, 1 mobile
Background: #1D1D1F
Text: #FFFFFF

/* Newsletter */
Input: 205px × 49.93px, radius: 12px, BG: #F0F1EC
Button: 118px × 49.93px, radius: 12px, BG: #06C167

/* Copyright */
Alignment: Centered
```

---

## Responsive Behavior

### Breakpoints
| Device | Breakpoint | Layout |
|--------|------------|--------|
| Mobile | 320px - 767px | Single column, hamburger menu |
| Tablet | 768px - 1199px | 2 columns, simplified navigation |
| Desktop | 1200px+ | Full layout, horizontal navigation |

### Grid Adaptations
| Section | Desktop | Tablet | Mobile |
|---------|---------|--------|--------|
| Brands | 5 logos | 3 logos | 2 logos |
| Features | 4 columns | 2 columns | 1 column |
| Products | 4 columns | 2 columns | 1 column |
| Highlights | 4 columns | 2 columns | 1 column |

### Navigation Behavior
```css
/* Desktop */
Horizontal menu, always visible

/* Tablet */
Horizontal menu, condensed spacing

/* Mobile */
Hamburger toggle, slide-down menu
Touch-friendly tap targets (44px minimum)
```

### Typography Scaling
| Element | Desktop | Tablet | Mobile |
|---------|---------|--------|--------|
| Hero Headline | 60px | 48px | 36px |
| Section Headers | 60px | 48px | 32px |
| Body Text | 16px | 16px | 14px |
| Button Text | 16px | 15px | 14px |

---

## Implementation Guidelines

### CSS Architecture
```css
/* Use CSS Custom Properties */
:root {
  --primary-green: #06C167;
  --light-bg: #F3FAFB;
  /* ... other tokens */
}

/* Mobile-first approach */
.component {
  /* Mobile styles */
  
  @media (min-width: 768px) {
    /* Tablet styles */
  }
  
  @media (min-width: 1200px) {
    /* Desktop styles */
  }
}
```

### Accessibility Requirements
- **Color Contrast**: Minimum 4.5:1 for normal text, 3:1 for large text
- **Focus Indicators**: Visible focus rings for all interactive elements
- **Keyboard Navigation**: All functionality available via keyboard
- **Screen Readers**: Proper ARIA labels and semantic HTML
- **Touch Targets**: Minimum 44px × 44px for interactive elements

### Performance Considerations
- Optimize images for web (WebP format with fallbacks)
- Implement lazy loading for below-fold images
- Minimize CSS and JavaScript bundle sizes
- Use efficient CSS selectors

### Browser Support
- **Chrome**: Last 2 versions
- **Firefox**: Last 2 versions  
- **Safari**: Last 2 versions
- **Edge**: Last 2 versions
- **Mobile**: iOS Safari, Chrome Mobile

### File Organization
```
css/
├── base/
│   ├── reset.css
│   ├── typography.css
│   └── variables.css
├── components/
│   ├── buttons.css
│   ├── cards.css
│   └── navigation.css
├── sections/
│   ├── hero.css
│   ├── features.css
│   └── footer.css
└── main.css
```

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2024-01-01 | Initial design system |
| 1.1 | 2024-01-15 | Added responsive specifications |
| 1.2 | 2024-02-01 | Updated color tokens and spacing |

---

**Maintained by**: Design Team  
**Last Updated**: 2024-01-01  
**Status**: Active
