## :root [**Back**](./../pseudoClass.md)

- `:root` is a CSS pseudo-class selector used to select the element that represents the root of the document.
- In HTML4, this is always the `<html>` element, since it is the highest-level ancestor of all other elements on the page. So, `:root` is identical(完全相同) to using the `html` as a selector, except that it has a higher specificity.

```css
:root {
    /** style the root element */
}

html {
    /** style the root element */
}
```

#### Case: learning `:root`

<p data-height="266" data-theme-id="21735" data-slug-hash="jWowoN" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/jWowoN/'>jWowoN</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- In document formats other than **HTML**, such as **SVG** and **XML**, the `:root` pseudo-class can refer to another higher-level ancestor.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>