# Web Design Assignment

This repository contains the solution for the web design assignment, consisting of a single HTML document (`index.html`) that adapts its layout based on two different CSS stylesheets (`styleA.css` and `styleB.css`).

## File Organization

The project structure is organized as follows in the root directory:

* `index.html`: The main HTML file containing the six box elements (A through F).
* `styleA.css`: The stylesheet for Version A, which arranges the boxes vertically using CSS Flexbox.
* `styleB.css`: The stylesheet for Version B, which arranges the first five boxes horizontally and fixes the last box to the bottom-right corner.

## Challenges They Faced

* **Maintaining Fixed Box Dimensions:** Ensuring that the boxes did not shrink or overlap when the browser window was resized required using `box-sizing: border-box` and `flex-shrink: 0` in Style A.
* **Preventing Horizontal Wrapping:** In Style B, keeping the first five boxes (A to E) strictly on a single line without wrapping down when the window became narrow was initially tricky, but it was resolved using `white-space: nowrap` and `display: inline-block`.
* **Fixed Positioning for the Last Element:** Positioning the final box (F) to stay permanently in the bottom-right corner of the window during scrolling and resizing required careful use of `position: fixed`.