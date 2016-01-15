## ::first-line [**Back**](./../pseudoClass.md)

- `::first-line` is a pseudo-element used to select the first formatted line in a block-level element (such as a paragraph `<p>`).
- Like `::first-letter`, the `::first-line` pseudo-element does not select the first line of an inline-level element; that is, an element that has `display: inline`. It only works on elements that have a display value of `block`, `inline-block`, `table-cell`, `table-caption`, or `list-item`.

#### Case: use first-of-type

```html
<div class="container">
    <article>
        <h2>Lorem Ipsum</h2>
        <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Cupiditate, voluptates, officiis esse adipisci fuga tempore iure vitae facilis quo id neque delectus perferendis maxime iusto in quam aliquid ratione nesciunt.
        </p>
        <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur, quam, sapiente fuga provident vero libero quae cum beatae suscipit rem similique vel eos cumque modi quo ad veritatis doloremque possimus!
        </p>
        <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nobis, nisi maiores repellendus delectus laboriosam ratione doloribus vero saepe deleniti reprehenderit minima officiis necessitatibus rem ab sint aperiam tenetur iure labore?
        </p>
    </article>
</div>
```

```css
p:first-of-type::first-line {
  text-transform: uppercase;
  text-decoration: underline;
  font-weight: bold;
  color: deepPink;
}

p::first-line {
  text-decoration: underline;
  text-transform: uppercase;
  font-weight: bold;
}
```
<p data-height="266" data-theme-id="21735" data-slug-hash="RrLWVr" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/RrLWVr/'>RrLWVr</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- The first line of a `table-cell` or `inline-block` cannot be the first formatted line of an ancestor element. So, in the following example, the first formatted line of the div is not the line "Hello".

```html
<div>
    <p style="display: inline-block">
        Hello
        <br>
        Goodbye
    </p> 
    etcetera
</div>
```

- Also note that the first line of the paragraph p in the following example doesn’t contain any letters (assuming the default style for `<br>`).

- There is an [old bug](https://code.google.com/p/chromium/issues/detail?id=129669) in Chrome that prevents [`text-transform`]() from being applied to the `::first-line` element.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>