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

```

```css
:disabled {
    background-color: #aaa;
    color: grey;
    border: 1px solid grey;
}
```

#### Note

- The `disabled` attribute is an **HTML5** attribute that can be set to the elements: `<button>`, `<input>`, `<textarea>`, `<optgroup>`, `<option>`, and `<fieldset>`.
- In comparison, `:enable` is to enable elements as a enable state.
- The `display` and `visibility` properties have no effect on the enabled/disabled state of an element, even if they are set to hide the element.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>