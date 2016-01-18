## :indeterminate [**Back**](./../pseudoClass.md)

- `:indeterminate` is a CSS pseudo-class selector used to select a user interface element that is in an indeterminate(未定的) state.
- More specifically, the :indeterminate pseudo-class selects the following elements:
    - Checkboxes (`<input type="checkbox">`) whose indeterminate attribute is set to true.
    - Radio buttons (`<input type="radio">`) whose radio button group contains no radio button that is checked.
    - A progress element (`<progress>`) that has no value attribute. The **progress element** is an HTML5 element that is used to represent the completion progress of a task.

#### Case:  nested boxes

- A checkbox can be either checked or unchecked. That's actually **literally(字面上)** true. Even if the checkbox's state is set to indeterminate, the checkbox's **visual style** will change, but the underlying state will still be either checked or unchecked.
- So, visually speaking, a checkbox can have three states: checked, unchecked, or indeterminate. (Again, the indeterminate state is visual only.)
- Using this concept, a checkbox can be checked if all its descendant checkboxes are checked, unchecked if all of its descendant checkboxes are unchecked, and indeterminate when only a subset of its descendant checkboxes are checked.

<p data-height="266" data-theme-id="21735" data-slug-hash="yePBMe" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/yePBMe/'>yePBMe</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- The indeterminate state of an element can be set **only via JavaScript**.
- The above state styles are applied in Chrome. Checkboxes usually look different in different browsers, and so do their state styles.

```html
<!-- doesn't work if you add it like so via HTML -->
<input type="checkbox" indeterminate>
```

```js
document.getElementByTagName('input')[0].indeterminate = true;
```

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>