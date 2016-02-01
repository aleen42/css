## :not() [**Back**](./../pseudoClass.md)

- `:not()` is a CSS negation pseudo-class selector. It is a functional pseudo-class selector that takes a **simple selector** as an argument, and then matches one or more elements that are **not represented** by the argument.
- The **simple selector** that `:not()` takes as an argument can be any of the following:
    - Type selector (eg. `span` etc.)
    - Class selector (eg. `.element`, `.sidebar` etc.)
    - ID selector (eg. `#element` etc.)
    - Pseudo-class selector (eg. `:first-child`, `last-of-type` etc.)
    - Attribute selector (eg. `[type="checkbox"]` etc.)
    - The universal selector (`*`)
- Invalid situation (**pseudo-element** and **negation pseudo-class** selector):

```css
/** Invalid */
p:not(:not(.same)) {}

p:not(:not(:last-child)) {}

:not(::first-letter) {}

a:not(::after) {}
```

- example:

```css
li:not(.new) {
    /** 
     * style all the list item except the one that 
       has the class new
     */
}
```

#### Case: learnning `:not()`

<p data-height="266" data-theme-id="21735" data-slug-hash="MKXxOM" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/MKXxOM/'>MKXxOM</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- The `:not()` selector can be chainable with more.

```css
artical:not(#feature):not(.header) {
    /** style the artical element match the situation */
}
```

- The `:not()` pseudo-class selector allows useless selectors to be written. For instance `:not(*)`, which represents no element at all will never apply any styles, or `foo:not(bar)` (e.g `p:not(article)`), which is equivalent to foo but with a higher specificity.
- Since you can use `:not()` globally and select all elements that are not represented by the argument, you should also note that `:not(X)` will match anything that isn't **X**, including **html** and **body**.
- Future levels of CSS (Level 4) will allow using selector lists inside `:not()`, such as `.title:not(h1, h2)` and `:not(#ID, .classname)`.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>