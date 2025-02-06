# CSS Cheat Sheet

## 1. Boilerplate CSS Setup
- Reset margin, padding, and box-sizing for all elements to ensure consistency across browsers.
- Set `html, body` to full width and height (`100%`).

---

## 2. Task 1: Box with Background Color
- `div` elements are often used to create boxes.
- Use `background-color` to apply a color.
- Text color is set with `color`.

**Reminder:** Avoid fixed units (`px`) when possible to ensure responsive design.

---

## 3. CSS Units Overview
### 1. `px` (Pixels)
- Absolute unit.
- Does not scale based on screen size.
- Useful for small, controlled elements but can lead to content overflow on smaller screens.

### 2. `%` (Percentage)
- Relative to the parent element.
- Width/height adjusts dynamically based on the parent container.

### 3. `vw` (Viewport Width) and `vh` (Viewport Height)
- `vw` is 1% of the viewport width.
- `vh` is 1% of the viewport height.
- Unlike `%`, these units are relative to the screen size, not the parent.

**Comparison:**
- `%` units scale based on the parent element.
- `vw` and `vh` scale based on the entire screen size.

### 4. `em`
- Relative to the font size of the current element.
- Example: If the font size is `15px`, `1em` equals `15px`.
- Multiples apply (e.g., `2em` = `30px`).

### 5. `rem`
- Relative to the root element's font size (`html`).
- Consistent scaling regardless of nesting.

**Key Difference:**
- `em` depends on the parent element's font size.
- `rem` depends on the root `html` font size.

---

## 4. Min and Max Width/Height
- Use `min-width` and `max-width` to create flexible designs that adapt to different screen sizes.
- `min-width` ensures the element does not shrink below a certain point.
- `max-width` prevents the element from expanding beyond a defined size.

**Example Insight:**
- If `width` is set to `600px` but `max-width` is `500px`, the element will not grow larger than `500px` even if the width is explicitly larger.

**Pro Tip:** Use `rem` for predictable scaling and avoid compounding effects from nested elements with `em`.

