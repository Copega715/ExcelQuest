---
name: ExcelQuest
colors:
  surface: '#faf9f8'
  surface-dim: '#dadad9'
  surface-bright: '#faf9f8'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f4f3f2'
  surface-container: '#efeeed'
  surface-container-high: '#e9e8e7'
  surface-container-highest: '#e3e2e1'
  on-surface: '#1a1c1c'
  on-surface-variant: '#404752'
  inverse-surface: '#2f3130'
  inverse-on-surface: '#f1f0ef'
  outline: '#717783'
  outline-variant: '#c0c7d4'
  surface-tint: '#0060ab'
  primary: '#005faa'
  on-primary: '#ffffff'
  primary-container: '#0078d4'
  on-primary-container: '#ffffff'
  inverse-primary: '#a3c9ff'
  secondary: '#455b9d'
  on-secondary: '#ffffff'
  secondary-container: '#a0b6fe'
  on-secondary-container: '#2f4686'
  tertiary: '#515f6c'
  on-tertiary: '#ffffff'
  tertiary-container: '#6a7885'
  on-tertiary-container: '#ffffff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d3e3ff'
  primary-fixed-dim: '#a3c9ff'
  on-primary-fixed: '#001c39'
  on-primary-fixed-variant: '#004883'
  secondary-fixed: '#dbe1ff'
  secondary-fixed-dim: '#b4c5ff'
  on-secondary-fixed: '#00174b'
  on-secondary-fixed-variant: '#2c4383'
  tertiary-fixed: '#d5e4f3'
  tertiary-fixed-dim: '#b9c8d7'
  on-tertiary-fixed: '#0f1d28'
  on-tertiary-fixed-variant: '#3a4854'
  background: '#faf9f8'
  on-background: '#1a1c1c'
  surface-variant: '#e3e2e1'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  title-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-code:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 8px
  sm: 16px
  md: 24px
  lg: 32px
  xl: 48px
  container-max: 1200px
  gutter: 20px
---

## Brand & Style

The design system is engineered to bridge the gap between corporate proficiency and engaging education. It adopts a **Corporate-Gamified** aesthetic, blending the structured reliability of financial software with the dopamine-driven feedback loops of modern learning apps.

The personality is authoritative yet encouraging—a "professional coach" persona. The UI employs a clean, high-contrast style that prioritizes clarity of data while using playful depth and motion to reward progress. Visuals utilize isometric iconography to give abstract financial concepts a tangible, toy-like quality, making complex formulas feel approachable.

## Colors

This design system uses a logic-driven palette rooted in the familiar ecosystem of data productivity.

- **Primary Blue (#0078D4):** Used for primary actions, progress indicators, and active states. It represents the "Action" layer.
- **Deep Navy (#002060):** Reserved for headers and persistent navigation. This provides a grounded, professional anchor to the lighter gamified elements.
- **Sky Blue (#E1F0FF):** Used for secondary backgrounds and subtle grouping, preventing visual fatigue during long study sessions.
- **Success Green (#107C10):** Specific to "Correct Answer" states, formula validation, and achievement badges.
- **Alert Red (#D83B01):** Specifically for syntax errors, incorrect answers, and critical warnings.

## Typography

The typography system relies on **Inter** for its exceptional legibility and neutral, professional tone. To support the specific needs of an Excel-based learning app, **JetBrains Mono** is introduced as a secondary functional font for formula entry and data strings, ensuring that characters like `0` and `O` or `1` and `l` are easily distinguishable.

Headlines use tight tracking and heavy weights to create a sense of accomplishment and impact. Body text maintains generous line heights to ensure readability during technical explanations.

## Layout & Spacing

The layout follows a **Fluid Grid** model with a 12-column structure for desktop and a single-column stack for mobile. 

- **Desktop:** 12 columns, 24px gutters, and 48px side margins.
- **Mobile:** 4 columns, 16px gutters, and 20px side margins.

The spacing rhythm is built on a 4px baseline grid. For gamified components like "Lesson Cards" or "Formula Builders," use `md` (24px) padding to create a sense of breathability and focus. Interactive elements should maintain a minimum tap target of 44x44px.

## Elevation & Depth

This design system uses a **Tonal & Physical Layering** approach to simulate a tactile learning environment.

1.  **Level 0 (Base):** Light gray background (`#F3F2F1`) for the main canvas.
2.  **Level 1 (Cards):** White surfaces with a "lifted" feel created by a 2px bottom border in a slightly darker shade of the surface color (simulating a physical button/card).
3.  **Level 2 (Pop-overs/Modals):** Soft, ambient shadows with a large blur radius (24px) and 8% opacity using the Primary Blue tint to suggest they are floating above the workspace.
4.  **Deep Headers:** The navigation bar uses the Navy (#002060) color without shadows, acting as a structural "ceiling" for the app.

## Shapes

The design system utilizes **Rounded (2xl)** geometry to lean into the friendly, gamified nature of the product.

- **Standard Components:** 1rem (16px) corner radius for buttons and input fields.
- **Large Containers:** 1.5rem (24px) corner radius for lesson cards, modals, and progress containers.
- **Data Cells:** Small 4px radius to maintain the "grid" feel of Excel without the sharpness of traditional spreadsheets.

## Components

### Buttons
Primary buttons use the "3D Tactile" style: a solid fill with a 4px darker bottom-border. On hover, the button translates 1px down; on active/click, it translates 4px down, "flattening" the shadow to give physical feedback of a press.

### Progress Bars
Heavy, 12px tall bars with fully rounded ends. The track is a light neutral (`#E1E1E1`) and the fill is a gradient of Primary Blue. For "Hot Streaks," the bar may transition to Success Green.

### Formula Input
A specialized text field using **JetBrains Mono**. It includes an "fx" prefix icon. Errors highlight the entire border in Alert Red and provide a floating tooltip anchored to the specific syntax error.

### Lesson Cards
Feature an isometric icon at the top right, a Title (md), and a progress indicator. They use the Level 1 elevation style with 24px padding.

### Chips & Badges
Small, pill-shaped markers used for "Difficulty Levels" (Basic, Advanced, Macro). These use low-contrast background tints of the primary colors with high-contrast text.

### Interactive Grids
Simplified spreadsheet views. Headers are Navy with white text. Selected cells use a 2px Primary Blue border with a 10% blue fill.