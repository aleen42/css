## :valid [**Back**](./../pseudoClass.md)

- `:valid` is a CSS pseudo-class used to select and style form `<input>` elements whose values validate according to their **type** specified in the type attribute.
- For example, email inputs (`<input type="email">`) whose values match a valid email address pattern.

#### Case: learning `:valid`

<p data-height="266" data-theme-id="21735" data-slug-hash="LNGPZE" data-default-tab="result" data-user="aleen42" class="codepen">See the Pen <a href="http://codepen.io/aleen42/pen/LNGPZE/">LNGPZE</a> by aleen42 (<a href="http://codepen.io/aleen42">@aleen42</a>) on <a href="http://codepen.io">CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- When a number input type (`<input type="number">`) is in the range of permitted values specified using the **min** and **max** attributes, then the `:valid` pseudo-class matches, and also the `:in-range` pseudo-class matches.
- Any styles applied using `:in-range` will override the styles applied using `:valid` only if the `:in-range` styles **come after** the `:valid` styles in the style sheet.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>