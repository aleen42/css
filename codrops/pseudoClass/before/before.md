## ::before [**Back**](./../pseudoClass.md)

- `::before` is a generated content element that represents a styleable abstract first child of the respective element.
- The content inserted using `::before` is inserted before other content inside the element and is displayed inline by default. The value of the content is specified using the [`content`]() property.

#### Case : add a quote before a block quote

```html
<blockquote>
    Your present circumstances don't determine where you can go; they merely determine where you start.—Nido Qubein
</blockquote>
```

```css
blockquote::before {
    content: "\201C"; /** style of the quote */
    color: deepPink;
    font-size: 3em;
    position: relative;
    top: 20px;
}
```

<p data-height="266" data-theme-id="21735" data-slug-hash="dGVYYB" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/dGVYYB/'>dGVYYB</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>



<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>