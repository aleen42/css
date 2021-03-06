## :disabled [**Back**](./../pseudoClass.md)

- `:disabled` is a pseudo-class selector used to select and style user interface elements (usually form elements) that are disabled.
- That is, it matches elements such as buttons (`<button>`), select menus (`<select>`), input types (`<input>`), and textareas (`<textarea>`), for example, that have the disabled attribute set and thus cannot be interacted with by the user.

```html
<input type="submit" disabled> <!-- disabled attribute added as a boolean value -->
<!-- OR -->
<input type="submit" disabled="disabled"> <!-- disabled attribute added with a "disabled" value -->
```

#### Case: chain selector with hover

```html
<input type="submit" value="Submit">
```

```css
:disabled {
    background-color: #aaa;
    color: grey;
    border: 1px solid grey;
}

input[type="submit"]:disabled:hover {
    cursor: not-allowed;
}
```

<p data-height="266" data-theme-id="21735" data-slug-hash="eJGBGW" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/eJGBGW/'>eJGBGW</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- The `disabled` attribute is an **HTML5** attribute that can be set to the elements: `<button>`, `<input>`, `<textarea>`, `<optgroup>`, `<option>`, and `<fieldset>`.
- In comparison, `:enabled` is to enable elements as a enabled state.
- The `display` and `visibility` properties have no effect on the enabled/disabled state of an element, even if they are set to hide the element.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>