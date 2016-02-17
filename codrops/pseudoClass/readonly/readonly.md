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



<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>