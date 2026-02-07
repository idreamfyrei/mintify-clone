# Mintlify Landing Page Recreation

A HTML and CSS powered recreation of the Mintlify documentation platform landing page.

##  Table of Contents
- [Overview](#overview)
- [Sections Recreated](#sections-recreated)
- [Technologies Used](#technologies-used)
- [Design System](#design-system)
- [Features](#features)
- [File Structure](#file-structure)
- [Getting Started](#getting-started)

##  Overview

This project is a faithful recreation of the Mintlify landing page, showcasing modern web design techniques including glassmorphism effects, smooth transitions, carousel, masks and filters and interactive components.

##  Sections Recreated

### 1. **Navigation Bar**
- Sticky navigation with glassmorphism backdrop effect
- Dropdown menus for "Resources" and "Documentation"
- Action buttons: "Contact sales" and "Start for free"
- Blur and hover effects on navigation items

### 2. **Hero Section**
- Prominent headline: "The Intelligent Knowledge Platform"
- "NEW" badge with pill design highlighting agent suggestions
- Email input with "Start now" call-to-action button
- Hero illustration/image mask

### 3. **Brand Logos Section**
- Logo grids of the brand logos

### 4. **Features Section** 
- Grid for cards of the section

### 5. **Carousel/Testimonials Section**
- Carousel with Customer success stories from brands
- caraousel cards with text clip, overflow control and hover effect
- Interactive carousel with navigation controls

### 6. **Pricing/CTA Section**

### 7. **Footer**
- Multi-column navigation menu
- Security badge section
- System status indicator with green dot
- Theme toggle buttons (System, Light, Dark)

##  Technologies Used

- **HTML5**: Semantic markup structure
- **CSS3**: Custom styling with modern features
- **Google Fonts**: Inter and Geist Mono font families
- **SVG Assets**: Vector graphics for icons and logos
- **Screenshot**: Images to replace animations

##  Design System

### Typography

#### Font Families
- **Primary Font**: `Inter` - Used for body text, headings, and most UI elements
  - Source: Google Fonts
  - Weights: 100-900 (variable)
  
- **Monospace Font**: `Geist Mono` - Used for code snippets and technical labels
  - Source: Google Fonts
  - Weights: 100-900 (variable)

#### Font Sizes
```css
--font-xsm: 0.75rem;     /* 12px - Small labels */
--font-sm: 0.875rem;     /* 14px - Secondary text */
--font-base: 1rem;       /* 16px - Body text */
--font-md: 1.125rem;     /* 18px - Medium text */
--font-lg: 1.25rem;      /* 20px - Large text */
--font-xl: 1.5rem;       /* 24px - Extra large */
--font-xxl: 2.5rem;      /* 40px - Section headings */
```

### Color Palette

#### Primary Colors
- **Background Main**: `lab(1.12% 0.14 -0.38)` - Near black (#08090a)
- **Background Secondary**: `#141516` - Greyish black for background of few sections
- **Text Primary**: `#ffffff` - Pure white
- **Text Secondary**: `#08090a` - Near black
- **Brand Color (Accent)**: `#18e299` - Bright teal/mint green
- **Muted Text**: `lab(100% 0 0 / 0.6)` - 60% opacity white

#### Additional Colors
```css
--color-background-hover: rgba(255, 255, 255, 0.055)
--color-border-soft: lab(100% 0 0 / 0.15)
--color-border-sub: lab(100% 0 0 / 0.07)
--color-text-soft: lab(100% 0 0 / 0.7)
```

### Spacing System
- **Base Unit**: `0.25rem` (4px)
- **Common Spacing**: Multiples of base unit (1x, 2x, 3x, 4x, 5x, 7x, 15x, 20x)
- **Container Widths**:
  - XL: `36rem` (576px)
  - 3XL: `48rem` (768px)
  - 4XL: `56rem` (896px)
  - 5XL: `64rem` (1024px)

### Border Radius
```css
--radius-sm: 0.25rem;    /* 4px */
--radius-md: 0.375rem;   /* 6px */
--radius-lg: 0.5rem;     /* 8px */
--radius-xl: 0.75rem;    /* 12px */
--radius-2xl: 1rem;      /* 16px */
--radius-3xl: 1.5rem;    /* 24px */
--radius-4xl: 2rem;      /* 32px */
```

##  Features

### Visual Effects
- **Glassmorphism**: Navigation bar with backdrop blur and transparency
- **Smooth Transitions**: All interactive elements have smooth hover states
- **Gradient Overlays**: Background gradients for depth and visual interest
- **Hover Effects**: 
  - Hero Image mask and filter to blend
  - Carousel cards dim on hover
  - Navigation links get rounded pill backgrounds
  - Buttons have brightness filters

### Interactive Components
- **Dropdown Menus**: Multi-column dropdown navigation
- **Carousel**: Customer testimonial carousel with prev/next controls
- **Form Input**: Email input with integrated CTA button
- **Badge Components**: Pill-shaped badges for highlighting new features


##  File Structure

```
project-root/
├── index.html              # Main HTML structure
├── style.css               # Complete stylesheet
├── resources/
│   ├── assets/             # logos of brand
│   ├── icons/              # icon svg of Mintlify
│   ├── brand_logo/         # Brand logos
│   └── landing_images/     # Screenshots of portions of landing pages
└── README.md               # Documentation
```

##  Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)

### Installation

1. Clone or download the project files
    ```bash
   git clone https://github.com/idreamfyrei/mintify-clone.git
   cd mintify-clone
   ```
2. Ensure the folder structure matches the layout above
3. Open `index.html` in your web browser using Live server or 
     ```bash
     # Node.js (with http-server)
     npx http-server
     ```
     Navigate to `http://localhost:8000`

### Deployment

Check the live deployment [here](https://mintify-clone.vercel.app/)


##  Customization

### Changing Colors
All colors are defined as CSS custom properties in the `:root` selector at the top of `style.css`. Modify these values to change the color scheme:

```css
:root {
  --font-color-primary: #your-color;
  --font-color-tertiary: #your-accent-color;
  /* etc. */
}
```

### Adjusting Typography
Font sizes and families can be modified in the CSS variables:

```css
:root {
  --font-inter: "Your Font", sans-serif;
  --font-base: 1rem; /* Adjust base size */
}
```

### Modifying Spacing
The spacing system is based on a multiplier of `0.25rem`:

```css
:root {
  --spacing: 0.25rem; /* Change base unit */
}
```

##  Key Design Patterns

1. **Glassmorphism Navigation**: Achieved using `backdrop-filter: blur()` with semi-transparent backgrounds
2. **Mask Gradients**: Used for smooth fade effects on background transitions
3. **Hover States**: Consistent pill-shaped backgrounds with blur effects
4. **Grid Layouts**: Flexible multi-column layouts for features and footer
5. **LAB Color Space**: Modern color definitions for better color accuracy

## Key Learnings
- Glassmorphism Effect
- Mordern way of defining global variable
- calc() function in CSS
- Masking on images
- Filter on components
- Few functionalities of webkit
- Text superimposed on images
- Grid and Flex applied together to get desired output

##  Screenshots

Mintify Demo
https://github.com/user-attachments/assets/239971a2-1846-4467-a400-7a2deb4d5981

---

**Created as a web development exercise to practice modern CSS techniques and semantic HTML structure.**
