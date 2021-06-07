# Design web pages with CSS

![CSS-Logo](https://icon-library.com/images/css-3-icon/css-3-icon-8.jpg)

## What is CSS?

* `CSS` stands for Cascading Style Sheets
* `CSS` describes how HTML elements are to be displayed on screen, paper, or in other media
* `CSS` saves a lot of work. It can control the layout of multiple web pages all at once

## What CSS does?

`CSS` is used to define styles for your web pages, including the design, layout and variations in display for different devices and screen sizes.

## CSS Syntax

```css
h1 {
    color:blue;
}
```

* h1: Selector
* color: Property
* blue: Value

## Ways to Insert CSS Into Our Webpages

1.  External `CSS` 

```html
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
```

2.  Internal `CSS`

```html
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
```

3.  Inline `CSS`

```html
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
```

## CSS Colors

***Colors*** are specified using predefined color **names**, **HEX**, **RGB**, or **RGPA**.

### How to define a color in CSS?

```css
section {
background-color: yellow; /*Name color*/
background-color: #000000; /*HEX color*/
background-color: rgb(100, 31, 70); /*RGP color*/
background-color: rgba(0, 68, 255, 0.5); /*RGPA color*/
}
```