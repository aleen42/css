## :not() [**Back**](./../pseudoClass.md)

- `:not()` is a CSS negation pseudo-class selector. It is a functional pseudo-class selector that takes a **simple selector** as an argument, and then matches one or more elements that are **not represented** by the argument.
- The **simple selector** that `:not()` takes as an argument can be any of the following:
    - Type selector (eg. `span` etc.)
    - Class selector (eg. `.element`, `.sidebar` etc.)
    - ID selector (eg. `#element` etc.)
    - Pseudo-class selector (eg. `:first-child`, `last-of-type` etc.)
    - Attribute selector (eg. `[type="checkbox"]` etc.)
    - The universal selector (`*`)
- Invalid situation (**pseudo-element** and **negation pseudo-class** selector):

```css
/** Invalid */
p:not(:not(.same)) {}


```


<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>