## :in-range [**Back**](./../pseudoClass.md)

- `:in-range` is a CSS pseudo-class used to style elements that have **range limitations** when the value that the element bound to is within the specified range limits.
- In other words, it matches an element when the value of its **value** attribute is within the range limitations specified on it.

```html
<input type="number" min="1" max="10" value="8">
```

```css
/*
 * As long as the value is between 1 and 10,
 * the input will match the :in-range selector and can be styled.
 */
input[type="number"]:in-range {
    /** styles here */
}
```

#### Note

- In comparison with `:in-range`, an element whose value is out of the specified range can be selected and styled using the `:out-of-range` pseudo-class selector.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>