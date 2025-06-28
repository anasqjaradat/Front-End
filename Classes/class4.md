# Lecture 4

[Back](../README.md)

## What We Learned

We covered the CSS **box model**:

* **Margin** – space outside the element.
* **Border** – the element's edge.
* **Padding** – space inside the border.
* **Div** – used to group and style content.

### Examples

#### Simple Box Example

```html
<!DOCTYPE html>
<html>
<head>
  <style>
    .box {
      margin: 20px;
      border: 5px solid #333;
      padding: 15px;
      background: lightgray;
    }
  </style>
</head>
<body>
  <div class="box">Styled box</div>
</body>
</html>
```

---

### Multiple Divs Example

```html
<!DOCTYPE html>
<html>
<head>
  <style>
    .container {
      width: 80%;
      margin: auto;
    }
    .section {
      margin: 20px 0;
      padding: 10px;
      border: 2px dashed blue;
      background: #f0f8ff;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="section">First section</div>
    <div class="section">Second section</div>
  </div>
</body>
</html>
```

---

### Summary

* Use **div** to structure and style content.
* Mastering **margin**, **border**, and **padding** is key for layout.
