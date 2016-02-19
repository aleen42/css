## :root [**Back**](./../pseudoClass.md)

- `:root` is a CSS pseudo-class selector used to select the element that represents the root of the document.
- In HTML4, this is always the `<html>` element, since it is the highest-level ancestor of all other elements on the page. So, `:root` is identical(完全相同) to using the `html` as a selector, except that it has a higher specificity.

```css
:root {
    /** style the root element */
}

html {
    /** style the root element */
}
```

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>