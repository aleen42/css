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
- 

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>