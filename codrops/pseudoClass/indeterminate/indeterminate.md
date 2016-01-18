## :indeterminate [**Back**](./../pseudoClass.md)

- `:indeterminate` is a CSS pseudo-class selector used to select a user interface element that is in an indeterminate(未定的) state.
- More specifically, the :indeterminate pseudo-class selects the following elements:
    - Checkboxes (`<input type="checkbox">`) whose indeterminate attribute is set to true.
    - Radio buttons (`<input type="radio">`) whose radio button group contains no radio button that is checked.
    - A progress element (`<progress>`) that has no value attribute. The **progress element** is an HTML5 element that is used to represent the completion progress of a task.


#### Note

- The indeterminate state of an element can be set **only via JavaScript**.

```html
<!-- doesn't work if you add it like so via HTML -->
<input type="checkbox" indeterminate>
```

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>