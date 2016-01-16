## :empty [**Back**](./../pseudoClass.md)

- `:empty` is a pseudo-class selector used to select elements in a page that are empty.
- An element counts as empty if it does not have any child elements (nodes) or text content. **Comments** and **processing instructions** do not affect whether the element is empty or not.
- Selecting empty elements is useful for hiding these elements because they may be the cause of weird(怪異的) vertical and/or horizontal white space if they have padding. It's also useful for removing empty elements in dynamic environments where empty elements are no longer needed or useful.

```html
<div><!-- comment --></div>
```

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>