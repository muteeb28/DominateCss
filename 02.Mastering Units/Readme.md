# 02. Mastering Units

## 1. Boilerplate CSS Setup
Before starting with units, it's important to set up a clean slate for styling. This ensures consistency across different browsers.

### **Steps:**
- Reset margin and padding to remove default spacing.
- Set `box-sizing: border-box;` so padding and borders are included in the element's total width and height.
- Ensure `html, body` take up the full width and height of the viewport.

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
html, body {
    width: 100%;
    height: 100%;
}
```

---

## 2. Task 1: Creating a Box with a Background Color
A **box** in HTML is usually made using a `<div>`. 

### **Steps to style a box:**
1. Use `background-color` to set the background color.
2. Use `color` to define the text color inside the box.

```css
.box {
    width: 200px;
    height: 100px;
    background-color: red; /* Box background color */
    color: white; /* Text color inside the box */
    display: flex;
    align-items: center;
    justify-content: center;
}
```

```html
<div class="box">Hello, World!</div>
```

📌 **Tip:** Avoid using fixed units (`px`) for width and height. Instead, prefer flexible units for better responsiveness.

---

## 3. Understanding CSS Units
CSS provides different units to define sizes, each with specific behaviors. Here’s a breakdown:

### **1. `px` (Pixels)**
- A fixed, absolute unit that does not change based on screen size.
- Best used for small elements like buttons or borders.
- Can cause layout issues on different screen sizes.

### **2. `%` (Percentage)**
- Relative to the parent element.
- Useful for fluid layouts that adjust dynamically.

### **3. `vw` (Viewport Width) and `vh` (Viewport Height)**
- `1vw` = 1% of the viewport’s total width.
- `1vh` = 1% of the viewport’s total height.
- Great for full-width sections and responsive elements.

**Comparison:**
- `%` adapts based on the parent element.
- `vw/vh` adapts based on the entire screen.

### **4. `em` (Relative to Parent Font Size)**
- 1 `em` = the font size of the current element.
- Example: If the parent font size is `16px`, then `2em` = `32px`.
- Can sometimes cause unwanted scaling due to nesting.

### **5. `rem` (Relative to Root Font Size)**
- 1 `rem` = the font size of the root element (`html`).
- More predictable than `em` because it doesn't depend on parent elements.

📌 **Key Difference:**
- `em` scales based on the parent element.
- `rem` scales based on the root font size.

---

## 4. Controlling Size with Min and Max Width/Height
To create adaptable designs, use:
- `min-width`: Ensures the element does not shrink below a specific size.
- `max-width`: Prevents the element from growing beyond a specific size.

### **Example:**
```css
.container {
    width: 600px;
    max-width: 500px; /* The element won’t exceed 500px even if width is 600px */
    min-width: 300px; /* Ensures it does not shrink below 300px */
}
```

📌 **Pro Tip:**
- Use `rem` for consistent scaling.
- Avoid using `em` inside nested elements to prevent unexpected growth.

---

By understanding these units, you’ll be able to create flexible and responsive web designs easily! 
