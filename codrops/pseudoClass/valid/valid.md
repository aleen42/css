## :valid [**Back**](./../pseudoClass.md)

- `:valid` is a CSS pseudo-class used to select and style form `<input>` elements whose values validate according to their **type** specified in the type attribute.
- For example, email inputs (`<input type="email">`) whose values match a valid email address pattern.

#### Note

- When a number input type (`<input type="number">`) is in the range of permitted values specified using the **min** and **max** attributes, then the `:valid` pseudo-class matches, and also the `:in-range` pseudo-class matches.
- Any styles applied using `:in-range` will override the styles applied using `:valid` only if the `:in-range` styles **come after** the `:valid` styles in the style sheet.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>