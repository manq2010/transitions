# transitions

CSS transitions let you animate a change from an element’s initial state to an end state.

The `transition` property, which is actually a shorthand property for `transition-property`, `transition-duration`, `transition-timing-function` and `transition-delay`

```css
button {
  /* ... other CSS properties ... */
  transition-property: background-color;
  transition-duration: 1s;
  transition-timing-function: ease-out;
  transition-delay: 0.25s;
}
```

* `transition-property` - This determines what CSS property will be transitioned. In this case it is the `background-color`.

* `transition-duration` - This determines the duration that the transition will occur over. In this case the color change will gradually happen over 1 second.

* `transition-timing-function` - This lets us change the speed of the transition over the course of its duration. Here it will `ease-out`, meaning the color change will be faster at the start than at the end of the transition.

* `transition-delay`- This determines the delay at which the transition will start. In this case, the color change starts a quarter of a second after the cursor rests on the button

The shorthand property looks like this:

```css
button {
  /* ... other CSS properties ... */
  background-color: white;
  transition: background-color 1s ease-out 0.25s;
}

button:hover {
  background-color: black;
}
```

### Performace

```css
div {
  width: 100px;
  height: 100px;
  transition: transform 2s 1s; 
}

div:hover {
  transform: rotate(180deg);
}
```

# CSS Cubic Bezier Generator

The [CSS Cubic Bezier Generator] will help you visualize how an transition is going to look. You can adjust the bezier curve my dragging the handles on the graph below, or, enter specific numbers into the cubic-bezier function. Once you've selected the perfect numbers, hit 'Compare Transitions' and this will show you how your transition compares to a few other popular transitions. Alter the speed and display for a different appearance. At the completion of the transition, just wait 1 second and you will see the animation in reverse.

[CSS Cubic Bezier Generator]: https://www.cssportal.com/css-cubic-bezier-generator/
