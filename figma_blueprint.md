# Figma Design Blueprint: Web Portfolio

This guide provides step-by-step instructions to recreate the "Data Science Portfolio" strictly adhering to the High-Contrast Dark Mode aesthetic.

## 1. Visual Style & Document Setup
- **Frame Size:** Desktop (1440px width x Auto height).
- **Global Background Color:** `#0b0f19` (Deep dark blue/black).
- **Layout Grid:** 
  - Type: Columns
  - Count: 12
  - Margin: 120px
  - Gutter: 24px

### Color Palette (Tokens)
- `bg-main`: `#0b0f19` (Main background)
- `bg-secondary`: `#131a28` (About & Contact section backgrounds)
- `bg-card`: `#1c2436` (Project cards & Skill badges)
- `text-primary`: `#f8fafc` (Headings & strong text)
- `text-secondary`: `#94a3b8` (Paragraphs)
- `accent-primary`: `#3b82f6` (Vibrant blue for buttons & links)
- `border-color`: `rgba(255, 255, 255, 0.1)`

## 2. Typography Guidelines
Use **Inter** or **Roboto** from Google Fonts.
- **H1/Slogan:** Inter, 64px, ExtraBold (800), Letter Spacing -2%. `text-primary` with `accent-primary` highlights.
- **Section Titles (H2/H3):** Inter, 40px, Bold (700). `text-primary`.
- **Intro Paragraph (Lead):** Inter, 18px, Regular (400), Line Height 160%. `text-secondary`.
- **Standard Body/Bio:** Inter, 16px, Regular (400), Line Height 160%. `text-secondary`.
- **Navigation/Buttons:** Inter, 16px, SemiBold (600).

## 3. Component Construction Guides

### A. The Header Component
1. Create a Frame (W: 100%, H: 80px).
2. Set Fill to `rgba(11, 15, 25, 0.85)` and add a **Background Blur** effect (12px).
3. Add a bottom border using `border-color`.
4. **Left Section (Auto Layout):**
   - Text node 1: "Abdelkareem Soliman & Renad Soliman" (Inter, 18px, Bold, `text-primary`).
   - Text node 2: "Senior Data Science Students" (Inter, 14px, Medium, `text-secondary`).
   - Group in Auto Layout: Vertical direction, 4px spacing.
5. **Right Section (Auto Layout):**
   - Text nodes for: Home, About, Skills, Projects, Contact. (Inter, 15px, Medium, `text-secondary`).
   - Group in Auto Layout: Horizontal direction, 32px spacing.

### B. The CTA Button Component
1. Add a Text layer: "View Our Graduation Project" (Inter, 16px, SemiBold).
2. Wrap in Auto Layout (`Shift + A`).
3. Set padding: 12px Top/Bottom, 28px Left/Right.
4. Set Fill to `accent-primary` (`#3b82f6`).
5. Set Corner Radius to 50px.
6. **Effect:** Add Drop Shadow: `rgba(59, 130, 246, 0.4)`, Y: 4, Blur: 14.

### C. Skill Badge Component
1. Create Auto Layout frame (Horizontal, 8px spacing, Align: Center).
2. Add an Icon (20x20px) and Text ("Python").
3. Set Fill to `bg-card` (`#1c2436`).
4. Set Stroke to `border-color`.
5. Set Padding: 8px Top/Bottom, 16px Left/Right.
6. Set Corner Radius to 50px.

### D. Project Card Component
1. Create a descriptive Frame (W: 350px, H: Auto). Wrap in Auto Layout (Vertical, 16px spacing, Padding: 40px).
2. Set Fill to `bg-card` (`#1c2436`).
3. Set Stroke to `border-color` (1px inside).
4. Set Corner Radius to 16px.
5. **Inner Elements:**
   - **Icon Container:** 60x60px Frame, Fill: `rgba(59, 130, 246, 0.1)`, Corner radius 12px. Add a 30x30px blue icon inside.
   - **Title Text:** "Ontology-Driven Machine..." (Inter, 22px, Bold, `text-primary`).
   - **Description Text:** "A smart manufacturing system..." (Inter, 16px, Regular, `text-secondary`).
   - **Link Container (Auto Layout, horizontal):** "Learn More" + Arrow icon (Inter, 16px, SemiBold, `accent-primary`).

## 4. Assembling the Layout (Desktop)
- **Hero Section:** Stack the Title, Paragraph, and CTA Button in a vertical Auto Layout container on the left side of the grid. Add a radial gradient circle in the background for a "glow" effect.
- **About/Skills:** Create a 2-column layout. Left column for Bio text, right column for a wrap-grid (Auto Layout with wrap enabled if using latest Figma) of Skill Badges.
- **Projects:** Create a Grid using Auto Layout (Horizontal, Wrap, 40px spacing) containing 2 Project Card instances.

## 5. Mobile Responsiveness (Auto Layout Check)
To design the mobile view:
- Change the main artboard width to 390px.
- Change header elements to stack vertically or use a hamburger menu wrapper.
- Change the About/Skills 2-column auto-layout to a vertical stack.
- Make Project Cards fill the parent container width (`Fill container` in Auto Layout settings).
