# CSS Transforms, Transitions, and Animations

## Transforms

The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

> 2d transform

Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.

![2d transform](https://lenadesign.org/wp-content/uploads/2020/02/skew.gif?w=580)

> 3d transform

Working with two-dimensional transforms we are able to alter elements on the horizontal and vertical axes, however there is another axis along which we can transform elements. Using three-dimensional transforms we can change elements on the z axis, giving us control of depth as well as length and width.

![2d transform](https://uicookies.com/wp-content/uploads/2019/01/3D-page-flip-css-page-transition.gif)

## Syntax

The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

```CSS
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}

```

## **Transitions & Animations**

![gif](https://cssanimation.rocks/images/posts/transitions-animations/transitions-animations.gif)

## Transitions

As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

![gif](https://miro.medium.com/max/856/1*OcsvgLF1jBw0WxCeMj4Mhw.gif)

There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.

>Example

```CSS
.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}
```

## Animations

Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off.

![gif](https://freefrontend.com/assets/img/css-animation-examples/CSS-Get-Attention-Animations.gif)

![gif](https://cdn.dribbble.com/users/1783374/screenshots/10100442/cute-loading.gif)

![gif](https://cdn.dribbble.com/users/215249/screenshots/2575539/octo-loader.gif)

To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

```CSS
@keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}
```
The animation above is named slide, stated directly after the opening @keyframes rule. The different keyframe breakpoints are set using percentages, starting at 0% and working to 100% with an intermediate breakpoint at 50%. The keywords from and to could be used in place of 0% and 100% if wished. Additional breakpoints, besides 50%, may also be stated. The element properties to be animated are listed inside each of the breakpoints, left and top in the example above.

It is important to note, as with transitions only individual properties may be animated. Consider how you might move an element from top to bottom for example. Trying to animate from top: 0; to bottom: 0; will not work, because animations can only apply a transition within a single property, not from one property to another. In this case, the element will need to be animated from top: 0; to top: 100%;.