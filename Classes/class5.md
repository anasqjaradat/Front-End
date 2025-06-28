
# Lecture 5

[Back](../README.md)

## What We Learned in HTML – Lecture 5

In this lecture, we covered:

* Meta tags
* Internal page navigation (bookmarks)
* Linking to sections on other pages
* Description lists (`<dl>`, `<dt>`, `<dd>`)
* Table structure using `colspan` and `rowspan`
* Using div containers for layout
* `z-index`
* `float`

---

### Meta Tags

Meta tags provide metadata about the HTML document and are placed within the `<head>` section.

```html
<head>
    <meta charset="UTF-8">
    <meta name="author" content="Your Name">
    <meta name="description" content="Description of the page">
</head>
```

---

### Internal Navigation (Same Page)

To link to a specific section within the same page, use an anchor tag with an `href` pointing to the `id` of the target element.

```html
<a href="#c4">Jump to Chapter 4</a>

<h2 id="c4">Chapter 4</h2>
```

---

### External Navigation (Other Pages)

To link to a specific section on a different page, append `#id` to the file name.

```html
<a href="html_demo.html#c4">Jump to Chapter 4</a>
<a href="../index.html#github">Jump to GitHub Section</a>
```

---

### Description Lists

A description list is a set of terms and their corresponding descriptions. It uses `<dl>` for the list, `<dt>` for each term, and `<dd>` for each description.

```html
<dl>
    <dt>Coffee</dt>
    <dd>Black hot drink</dd>
    <dt>Milk</dt>
    <dd>White cold drink</dd>
</dl>
```

---

### Tables with `colspan` and `rowspan`

You can span columns and rows in a table to create more flexible layouts.

```html
<table>
    <tr>
        <th colspan="2">Name</th>
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td rowspan="2">50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
    </tr>
</table>
```

---

### Div Containers Example

Using div elements with IDs can help organize sections of your page for layout or styling purposes.

```html
<div id="checkAbsolute">
    <div id="Top">Top</div>
    <div id="Bottom">Bottom</div>
</div>
```

This structure creates two sections named "Top" and "Bottom" inside a container `checkAbsolute`.

---

### `z-index`

The `z-index` property in CSS controls the vertical stacking order of elements that overlap. Higher `z-index` values appear on top of lower ones. It only works on elements that have a `position` value other than `static`.

```html
<style>
  .box1 {
    position: absolute;
    top: 20px;
    left: 20px;
    width: 100px;
    height: 100px;
    background-color: red;
    z-index: 1;
  }

  .box2 {
    position: absolute;
    top: 40px;
    left: 40px;
    width: 100px;
    height: 100px;
    background-color: blue;
    z-index: 2;
  }
</style>

<div class="box1"></div>
<div class="box2"></div>
```

---

### `float`

The `float` property allows elements to be positioned to the left or right of their container, with text and inline elements flowing around them.

```html
<style>
  .float-left {
    float: left;
    width: 150px;
    margin-right: 15px;
  }
</style>

<img src="image.jpg" alt="Sample" class="float-left">
<p>
  This paragraph wraps around the image. The image floats to the left, and the text flows next to it. This technique is often used for text-wrapped images or sidebars.
</p>
```

To clear floated elements (so that following content doesn’t wrap), you can use:

```html
<div style="clear: both;"></div>
```