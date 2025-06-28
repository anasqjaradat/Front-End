# Lecture 3

[Back](../README.md)

## What We Learned in CSS

CSS can be added to HTML documents in 3 ways:

- Inline - by using the style attribute inside HTML elements
- Internal - by using a `<style>` element in the `<head>` section
- External - by using a `<link>` element to link to an external CSS file

### EXAMPLES

- **inline style**
Inline CSS is used to apply a unique style to a single HTML element.

```html
<h1 style="color:blue;">A Blue Heading</h1>

<p style="color:red;">A red paragraph.</p>
```

- **Internal style**
An internal CSS is used to define a style for a single HTML page.

```html

<!DOCTYPE html>
<html>
    <head>
        <style>
            /* used for style the full tag  */
            h1{color: rgb(36, 207, 207);font-size: 40px;}
            /* id */ 
            #github{
                color: black;
                font-size: 10px;
                background-color: aliceblue;
            }
            /* class */
            .bluelink{
                color: blue;
                font-size: small;
                background-color: aqua;
            }
        
        </style>
    </head>
<body>

    <h1>This is a heading</h1>
    <!--  id  -->
    <a id="github" href="https://github.com/anasqjaradat/Front-End" target="_blank" >Go To My Github</a>
    <!-- class  -->
    <a class="bluelink" href="/Classes/class3.md">Link</a>
</body>
</html>
```

- **External style**
An external style sheet is used to define the style for many HTML pages.

html

```html
<!DOCTYPE html>
<html>
    <head>
      <link rel="stylesheet" href="styles.css">
    </head>
<body>

    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>
</body>
</html>
```

css

```css
body {
  background-color: powderblue;
}
h1 {
  color: blue;
}
p {
  color: red;
}
```
