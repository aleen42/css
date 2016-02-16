## :only-of-type [**Back**](./../pseudoClass.md)

- `:only-of-type` is a CSS pseudo-selector which matches an element if its parent has no other children **of the same type**.
- For example, `p:only-of-type` will match a paragraph only if it is the only paragraph inside its parent. So, it will select the following paragraph:

```html
<article>
    <h1>Heading</h1>
    <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Soluta, enim, libero voluptatum id nostrum porro laborum error nisi fugit atque a possimus ullam maxime quia tenetur obcaecati dolorum dolore placeat.
    </p>
</article>
```

#### Case: learning `:only-of-type`

<p data-height="266" data-theme-id="21735" data-slug-hash="EPMEzo" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/EPMEzo/'>EPMEzo</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- `:only-of-type` is familiar with `:only-child`.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>