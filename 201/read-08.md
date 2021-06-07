# CSS Layout

CSS page layout techniques allow us to take elements contained in a web page and control where they are positioned relative to their default position in normal layout flow, the other elements around them, their parent container, or the main viewport/window.

![css layout](/gallery/layout.jpg)

## Building Blocks

> Block-level elements: start on a new line

![Block-level](/gallery/Block-level.jpg)

> Inline elements: flow in between surrounding text

![Inline](/gallery/Inline.jpg)

> Containing Elements: If one block-level element sits inside another block-level element then the outer box is
known as the containing or parent element.

![Containing](/gallery/Containing.jpg)

## Controlling the Position of Elements

> Normal flow: Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. Even if you specify the width of the boxes and there is space for two elements to sit side-byside, they will not appear next to each other.

> Relative Positioning: This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position they would be in in normal flow.

> Absolute positioning: This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position
of any surrounding elements (as they simply ignore the
space it would have taken up). Absolutely positioned elements
move as users scroll up and down the page.

> Fixed Positioning This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element. Elements with fixed positioning do not affect the position of surrounding elements and they do not move when the user scrolls up or down the page.

> Floating Elements Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow.

![positions](https://cdn.educba.com/academy/wp-content/uploads/2019/12/CSS-Position-768x428.jpg.webp)

## Screen size

![size](https://assets.codepen.io/17824/internal/screenshots/pens/EBbxp.default.png?fit=cover&format=auto&ha=false&height=540&quality=75&v=2&version=1360004161&width=960)

## Page size

> Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).

## Layout grids

![Grids](https://www.bitdegree.org/learn/storage/media/images/f2804b75-5393-4504-bad9-fec3f56dfb94.png)

> Grids help create professional and flexible designs.

> CSS Frameworks provide rules for common tasks.

>You can include multiple CSS files in one page.
