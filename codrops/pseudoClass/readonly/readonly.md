## :read-only [**Back**](./../pseudoClass.md)

- `:read-only` is a CSS pseudo-class selector that matches any element that does not match the `:read-write` selector.
- In other words, it matches elements that are not editable by the user. Elements that fall into the editable category include:
    - `<input>` elements (of any type) that are **not read-only** and that are **not disabled**.
    - `<textarea>`s that are neither read-only nor disabled (similar to the inputs).
    - Any other element that is not an `<input>` or a `<textarea>`, and that has the contenteditable attribute set.
- The `:read-only` pseudo-class selector matches any element that is **not one of the above**.
- The following are examples of elements that can be selected using `:read-only`:

```html
<input type="text" disabled>

<input type="number" disabled>

<input type="number" readonly>

<textarea name="nm" cols="30" rows="10" readonly></textarea>

<div class="random"></div>
```

#### Case: test `:read-only`

<p data-height="266" data-theme-id="21735" data-slug-hash="PZgGGY" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/PZgGGY/'>PZgGGY</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- The `:read-only` selector is not supported in **Internet Explorer** and on **Android**.
- In Chrome, Firefox, Safari, and Opera, inputs that are **disabled** (have the disabled attribute set) are treated as **read-write** not as read-only, unlike what the spec says. So, disabled elements will not match :read-only in these browsers even if they should.
- In Opera, elements that are editable using the **contenteditable** attribute are treated as **read-only** because it does not support the contenteditable attribute.
- 

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>