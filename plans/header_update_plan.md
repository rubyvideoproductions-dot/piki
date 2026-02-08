# Header Positioning Update Plan

## Objective
Change the behavior of the top navigation bar so that it stays at the top of the document (scrolls away) rather than staying fixed to the viewport (sticky).

## Files to Modify

### 1. `css/style.css` (affects `index.html`)
- **Target Selector**: `.header` (Line ~110)
- **Change**: Replace `position: fixed` with `position: absolute`.
- **Reason**: This will position the header at the top of the `<body>`, allowing it to scroll out of view when the user scrolls down.

### 2. `contact.html` (Internal Styles)
- **Target Selector**: `.header` (Line ~200 inside `<style>`)
- **Change**: Replace `position: fixed` with `position: absolute`.
- **Reason**: Same as above, ensuring consistent behavior across the site.

## Verification
- Open `index.html` and `contact.html` in a browser.
- Scroll down the page.
- Verify that the navigation bar moves up and disappears as you scroll, rather than staying stuck to the top of the window.
