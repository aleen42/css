## :blank [**Back**](./../pseudoClass.md)

- `:blank` is a CSS pseudo-class selector used to select pages of a printed document, such as a book, that are empty as a result of a forced **page break**.
- It is used in conjunction with the `@page` rule which selects all pages in a printed document. So, when used with `@page`, `:blank` acts kind of like a filter used to select only the empty pages that are empty as a result of a forced **page break**.

```css
@page :blank {
    /** styles for the empty page */
}

```

#### Note

- Only the **left** and **right** values of the `page-break-before` and `page-break-after` properties can generate pages that match `:blank`.
- Styles specified in a `:blank` `@page` rule override any styles provided in an `@page` rule that has no pseudo-class specified.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>