## :read-write [**Back**](./../pseudoClass.md)

- `:read-write` is a CSS pseudo-class selector that matches elements that are **editable** by the user.
- Elements that fall into the editable category include:
    - `<input>` elements (of any type) that are **not read-only** and that are **not disabled**.
    - `<textarea>`s that are neither read-only nor disabled (similar to the inputs).
    - Any other element that is not an `<input>` or a `<textarea>`, and that has the contenteditable attribute set.
- The following are examples of elements that can be selected using `:read-write`:

```html
<input type="text">

<input type="number">

<textarea name="nm" id="id" cols="30" rows="10"></textarea>

<div class="random" contenteditable></div>
```

#### Note

- In Chrome, Firefox, Safari, and Opera, inputs that are **disabled** (have the disabled attribute set) are still treated as **read-write**, unlike what the spec says.
- In Opera, elements that are editable using the **contenteditable** attribute are treated as **read-only** because it does not support the contenteditable attribute.
- In Chrome, elements editable using the **contenteditable** attribute do not match `:read-write`, and hence are not selected with `:read-write`. They don't match the `:read-only` selector either, how they are treated is unknown. Same applies to regular elements that are not editable with contenteditable, they don't match either of the two pseudo-class selectors.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>