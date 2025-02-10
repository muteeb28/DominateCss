# 01. Setup and Basics

## 1. CSS Boilerplate (Universal Reset)
### **Purpose**
Ensure a consistent baseline by resetting margins, paddings, and setting universal box-sizing.

### **Key Properties**
```css
* {
    margin: 0; /* Removes default margins */
    padding: 0; /* Removes default padding */
    box-sizing: border-box; /* Includes padding and border in the element's total width and height */
}
html, body {
    width: 100%; /* Ensures full page coverage */
    height: 100%;
}
```

## 2. Box Creation and Styling
### **Task:** Create a box with a red background.

### **Key Concept**
- A box is typically created using a `<div>` element.
- `background-color` is used to set the box color.
- `color` is used to change the text color.

### **Example**
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

## 3. Core CSS Properties for Box Model
### **Essential Properties**
- `width` & `height`: Controls the size of the element.
- `background-color`: Sets the background color.
- `color`: Defines the text color inside the element.

## 4. Key CSS Concepts
### **Box Model**
Understanding how elements are sized and spaced:
```
[ Margin ]
   [ Border ]
      [ Padding ]
         [ Content ]
```
- `width`, `height` → Define the content size.
- `padding` → Adds space inside the border.
- `border` → Defines the element boundary.
- `margin` → Creates space outside the element.

### **Selectors**
- **Class Selector**: Targets elements with a specific class.
  ```css
  .classname {
      color: blue;
  }
  ```
- **Universal Selector**: Applies styles to all elements.
  ```css
  * {
      box-sizing: border-box;
  }
  ```

## Notes
- **A box in HTML = `<div>`**
- **Use `background-color` for background and `color` for text.**
- **Boilerplate CSS ensures uniform styling across browsers.**


