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

#### Note

- In document formats other than **HTML**, such as **SVG** and **XML**, the `:root` pseudo-class can refer to another higher-level ancestor.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>