---
title: "From Static to Active: Using CSS Transforms"
author: Tarun Balaji Ravi
description: "Using CSS transform property functions "
date: 2022-11-27T20:32:52.810Z
tags:
  - post
  - css
  - translation
  - functions
image: /assets/blog/translation.png
imageAlt: Translation Functions
---
## 2D Translation Functions

With so many stale, static websites out there on the web, the CSS transform property is an easy way to add lively motion to your webpages. There are many functions that can be used as values for the transform property. We will be looking at the four basic, yet powerful ones: skew, rotate, translate, and scale. These are the 2D translation functions that can be used with CSS transform. 

First up is the *skew( )* function. The skew function allows you to either tilt an element to the left or right, up or down, or both at the same time. To tilt an element to the left or right, which would be along the x-axis, use *skewX( )*. Passing a positive value to the *skewX* function will skew the element to the right, while passing a negative value will skew the element to the left. To skew an element up or down, use *skewY( )*. A positive value will skew it down, and a negative value will skew it up.

```
.element {
 transform: skewX(40deg);
}

```
```
.element {
 transform: skewY(-25deg);
}

```

You can the *skew( )* shorthand function to skew an element along both the x-axis and y-axis. The first value passed will skew the element along the x-axis and the second value will tilt the element along the y-axis. Just like the *skewX( )* and *skewY( )* functions, the positive value will skew the element to the right, while a negative value will skew the element left. A positive value passed second will skew the element down, and a negative value passed second will skew the element up.

```
.element {
 transform: skew(40deg, 40deg);
}

```

Up next, we have the *rotate( )* function. To rotate, simply pass a value in degrees using the deg unit. A positive value will rotate the element to the right, while a negative value will rotate the element to the left.

```
.element {
 transform: rotate(360deg);
}

```
```
.element {
 transform: rotate(-360deg);
}

```

In addition, you can also use the turn unit instead of degrees. A turn with a value of 1 is equal to a rotation of 360 degrees. For example, if you wanted to tilt an element slightly to the right, you can pass a value of 0.3turn to the rotate function. Just like using degrees, a positive turn value will rotate the element to the right, while a negative turn value will rotate the element to the left. 

```
.element {
 transform: rotate(0.3turn);
}

```

For our third 2D translation function, we have the *translate( )* function. Using this function, we can move an element along the x-axis, which would move it right or left, and along the y-axis, which would move it up or down. 

To move an element along the x-axis, the *translateX( )* function is used. Passing a positive value will move the element to the right, while passing a negative value will move an element to the left. To move an element along the y-axis, the *translateY( )* function is used. Passing a positive value will move the element down, while passing a negative value will move the element up. 

```
.element {
 transform: translateX(20px);
}

```
```
.element {
 transform: translateY(-10px);
}

```

A shorthand to combine both x and y translates is the *translate( )* function. The first value passed with translate the element along the x-axis, and the second value will translate the element along the y-axis. Just like the other translate functions, a positive value will move the element right, and a negative value will move the element left. Passing a positive second value will move the element down and passing a negative second value will move the element up. 

```
.element {
 transform: translate(20px, 20px);
}

```

It should be noted that the *translate( )* function does not change an elements in-flow position. Therefore, it has no effect on the layout algorithms such as flexbox or grid. 

Further, any length value can be passed to the *translate( )* function. You can even use a percentage value, and the percentage refers to the size of the element itself, which allows you to move the element right outside of another one. Using a positive value, such as 100%, will move the element to the right, while a negative value, such as -100%, will move the element to the left. Passing a positive percentage for the second value will translate the element down and passing a negative percentage for the second value will translate the element up. 

```
.element {
 transform: translate(100%, -100%);
}

```

One great aspect of the translate function is that it is hardware accelerated. 😊 

Lastly, the *scale( )* function can used to affect the size of an element. Note that using the scale function will apply the re-sizing to the font-size, padding, height, and width of an element. The *scaleX( )* function can be used to affect the width of an element and the *scaleY( )* function can be used to affect the height of an element. The *scale( )* shorthand function allows you to change the size of both the width and height, with the first value passed stretching the element horizontally, affecting its width, and the second value passed stretching the element vertically, affecting its height. 

```
.element {
 transform: scale(1.2);
}

```

Now that you have learned some basic, yet powerful functions for the CSS transform property, I hope you can start incorporating them into your webpages to make them livelier. To recap, the *skew( )* function tilts an element to the right or left, or up or down, the *rotate( )* function rotates an element from its current position, the *translate( )* function moves an element to the right or left, or up or down, and the *scale( )* function affects the size of the element. Go have fun using CSS transforms!

## Codepen Embed

<figure>

<iframe height="300" style="width: 100%;" scrolling="no" title="Translation Functions Codepen" src="https://codepen.io/tarunbalaji3/embed/LYrQoLy?default-tab=html%2Cresult" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/tarunbalaji3/pen/LYrQoLy">
  Translation Functions Codepen</a> by tarunbalaji3 (<a href="https://codepen.io/tarunbalaji3">@tarunbalaji3</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

<figcaption>
Translation Functions (inspired by <a href='https://codepen.io/team/css-tricks/pen/povNBmQ'>@css-tricks</a>)
</figcaption>
</figure>

