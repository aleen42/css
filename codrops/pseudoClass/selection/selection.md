## ::selection [**Back**](./../pseudoClass.md)

- `::selection` CSS pseudo-element represents a portion() of the document that is highlighted by the user. For example, a portion of a page that is selected by the user using the mouse or any other pointing device.

#### Case: add search... to a search bar

```html
<input type="text" placeholder="search...">
```

```css
input::-webkit-input-placeholder {
    color: #999;
}

::-moz-placeholder {
    color: #999;
}

:-ms-input-placeholder {
    /** notice that ie has only a single colon) */
    color: #999;
}

::-webkit-input-placeholder {
    color: #999;
}

::placeholder {
    color: #999;
}
```

<p data-height="266" data-theme-id="21735" data-slug-hash="BjwoJR" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/BjwoJR/'>BjwoJR</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>