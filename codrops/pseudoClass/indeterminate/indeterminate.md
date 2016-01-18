## :indeterminate [**Back**](./../pseudoClass.md)

- `:indeterminate` is a CSS pseudo-class selector used to select a user interface element that is in an indeterminate(未定的) state.
- More specifically, the :indeterminate pseudo-class selects the following elements:
    - Checkboxes (`<input type="checkbox">`) whose indeterminate attribute is set to true.
    - Radio buttons (`<input type="radio">`) whose radio button group contains no radio button that is checked.
    - A progress element (`<progress>`) that has no value attribute. The **progress element** is an HTML5 element that is used to represent the completion progress of a task.

#### Case:  nested boxes

- A checkbox can be either checked or unchecked. That's actually **literally(字面上)** true. Even if the checkbox's state is set to indeterminate, the checkbox's visual style will change, but the underlying state will still be either checked or unchecked.

#### Note

- The indeterminate state of an element can be set **only via JavaScript**.

```html
<!-- doesn't work if you add it like so via HTML -->
<input type="checkbox" indeterminate>
```

```js
document.getElementByTagName('input')[0].indeterminate = true;
```

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>