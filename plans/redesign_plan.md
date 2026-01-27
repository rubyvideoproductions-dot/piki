# Redesign Plan: Typographic Dark Minimalist

## 1. Vision
Transform the landing page into a minimal, dark, typographic experience inspired by the "Folio:06" aesthetic. The initial view will be a full-screen typographic cover, followed by the showreel.

## 2. Structure & Layout

### A. New "Typographic Cover" (Hero Section)
*   **Dimensions:** 100vh (Full Viewport Height).
*   **Background:** Visible Three.js/WebGL dark gradient (ensure transparency/layering allows it to shine through).
*   **Grid Layout:** 3-column x 3-row (approximate) or Flexbox with absolute positioning for corners.

#### UI Elements
*   **Top Bar (Flex/Grid):**
    *   Left: "FOLIO:06" (Placeholder, recommend: `PEAK:2026`)
    *   Center: "JONAS REYMONDIN" (Placeholder, recommend: `PEAK STUDIOS`)
    *   Right: "©2026"
*   **Center Stage:**
    *   Large, centered, uppercase sans-serif typography.
    *   Text: "YOUR GOALS. OUR SPARK. PEAK RESULTS. ADAPTIVE CREATIVE PROFESSIONAL EFFICIENT."
    *   Style: Bold/Heavy weight, clean lines.
*   **Bottom Bar (Flex/Grid):**
    *   Left: "AVAIL: 04.2026"
    *   Center: "CONTACT" (Link/Button)
    *   Right: "10:29:18 PM, FR" (Real-time clock or static placeholder)
*   **Decorative:**
    *   Corner/Side markers (`+`) at grid intersections or viewport edges.

### B. Showreel Section
*   **Placement:** Immediately following the Typographic Cover (scroll down).
*   **Transition:** Smooth scroll or reveal.
*   **Content:** The existing video card component.

## 3. Visual Style
*   **Theme:** Dark (Background `#0a0408` or similar from `style.css`).
*   **Typography:**
    *   Font: Inter (existing).
    *   Case: Uppercase.
    *   Color: White / Off-white.
    *   Alignment: Center (for main text), Justified/Spread (for bars).

## 4. Implementation Steps

### Phase 1: Setup & Cleanup
1.  [ ] Update `index.html` to remove inline light-theme styles and defer to `style.css`.
2.  [ ] Ensure `style.css` dark theme is active.

### Phase 2: HTML Structure
3.  [ ] Create new `<section id="hero-cover">` container.
4.  [ ] Implement the Top Bar, Center, and Bottom Bar structure within `#hero-cover`.
5.  [ ] Move the existing Showreel/Video component to a new `<section id="showreel">` below the cover.

### Phase 3: Styling (CSS)
6.  [ ] Implement Grid/Flex layout for the cover.
7.  [ ] Style the typography (size, spacing, weight) to match the reference "minimalist" look.
8.  [ ] Add the decorative `+` markers.
9.  [ ] Ensure the Three.js background is visible behind the text.

### Phase 4: Content & Logic
10. [ ] Insert the specific text: "Your Goals. Our Spark..."
11. [ ] Implement simple JS clock for the bottom right corner.
