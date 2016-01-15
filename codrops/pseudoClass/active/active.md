## :active [**Back**](./../pseudoClass.md)

- `:active` is a CSS pseudo-class. It specifies and selects an element based on a state—the active state—and is used to apply styles to an element when it matches that state.

```css
::selection {
    background-color: #222;
    color: white;
}

::-moz-selection {
    background-color: #222;
    color: white;
}

blockquote::selection {
    background-color: #aaa;
    color: white;
}
```

<p data-height="266" data-theme-id="21735" data-slug-hash="dGVGyp" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/dGVGyp/'>dGVGyp</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- Only a subset of all CSS properties can be used to style a `::selection`:

categories|items
----------|-----
**Color Properties**|`color`, `background-color`, and `text-shadow` properties.

- The `::selection` pseudo-element was drafted for CSS Selectors Level 3 but was removed before it reached the Candidate Recommendation status, and it is currently not part of any CSS module on the standards track. However, it is still implemented in most browsers, and is likely to remain so.
- Using `text-shadow` in ::selection is only supported in Chrome, Safari, Opera, nd Firefox.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>