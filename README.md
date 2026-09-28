# Assignment 2

A single HTML page with two different CSS layouts. The page contains six boxes labeled A to F and uses only HTML and CSS.

## Files

- `index.html`: The page structure and the six boxes.
- `styleA.css`: A vertical layout with centered boxes and alternating colors.
- `styleB.css`: A horizontal layout with hover colors and box F fixed in the bottom-right corner.

## How to view

Open `index.html` in a browser. Style A is selected by default.

To view Style B, change the stylesheet link in `index.html` to:

```html
<link rel="stylesheet" href="styleB.css">
```

Save the file and refresh the browser. Change the filename back to `styleA.css` to view Style A again.

## Layout challenges

- In Style A, the spaces between boxes need to change with the window height without shrinking the boxes. Flexbox, `justify-content: space-between`, and `flex-shrink: 0` handle this. A minimum gap keeps boxes apart on short windows, where the page can scroll.
- In Style B, boxes A to E must stay on one row even in a narrow window. `flex-wrap: nowrap` and `flex-shrink: 0` keep their positions and sizes.
- Box F needs to stay in the bottom-right corner in Style B. `position: fixed` keeps it attached to the window.
