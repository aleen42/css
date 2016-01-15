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


<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>