## ::placeholder [**Back**](./../pseudoClass.md)

- `::placeholder` is a CSS pseudo-element that represents placeholder text in an `input` field—text that represents the input and provides a hint to the user on how to fill out the form.

#### Case: add YYYY/MM/DD to clarify

```html
<input type="date" placeholder="DD/MM/YYYY">
```

```css
input::-webkit-input-placeholder {
  color: #999;
}

::-moz-placeholder {
  color: #999;
}

:-ms-input-placeholder {
  color: #999;
}

::-webkit-input-placeholder {
  color: #999;
}

::placeholder {
  color: palevioletred;
}
```

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>