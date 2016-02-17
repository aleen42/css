## :out-of-range [**Back**](./../pseudoClass.md)

- `:out-of-range` is a CSS pseudo-class used to style elements that have range limitations when the value that the element bound to is outside the specified range limits.
- Examples of elements with range limitations are sliders and inputs that accept a number as a value. For example:

```html
<input type="number">
```

- Such an input would have a range of acceptable values specified using the min and max attributes. The value attribute would hold the current value of the input.

```html
<input type="number" min="1" max="10" value="8">
```

- In this example, if the value exceeds the range limitations, the input will match the :out-of-range selector. The following will style the input when its value it outside the range limit:

```css
input[type="number"]:out-of-range {
    /* styles here */
}
```

#### Case: learning `:out-of-range`

<p data-height="266" data-theme-id="21735" data-slug-hash="qbwadK" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/qbwadK/'>qbwadK</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>