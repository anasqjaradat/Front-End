
# Online

[Back](../README.md)

## What We Learned in CSS – Lecture 7

In this lecture, we covered:

* CSS Grid layout basics
* Defining rows and columns
* Styling grid items
* Responsive spacing with `gap`

---

### CSS Grid Overview

CSS Grid is a powerful layout system that allows you to create complex web layouts with ease by defining rows and columns.

---

### Basic Grid Structure

```html
<div class="grid-container">
  <div class="grid-item">1</div>
  <div class="grid-item">2</div>
  <div class="grid-item">3</div>
  ...
</div>
```

```css
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  grid-template-rows: 150px 150px 150px;
  gap: 20px;
  padding: 20px;
  background-color: #f0f0f0;
}
```

---

### Styling Grid Items

Each grid item is styled to look neat and centered.

```css
.grid-item {
  background-color: #4CAF50;
  color: white;
  font-size: 24px;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 8px;
}
```

---

### Visual Result

You get a **3×3 grid layout** with numbered blocks. Each block is:
- 150px tall
- Centered with flexbox
- Separated by a 20px gap

---

### Key Properties Used

- `display: grid`: Enables grid layout on the container.
- `grid-template-columns`: Defines the number and width of columns.
- `grid-template-rows`: Defines the number and height of rows.
- `gap`: Sets spacing between rows and columns.
- `padding`: Adds space inside the container.

---

Would you like to expand this layout using:
- `grid-column` / `grid-row` for spanning cells
- `grid-template-areas` for named layout zones
- Media queries for responsiveness
