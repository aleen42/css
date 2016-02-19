## :right [**Back**](./../pseudoClass.md)

- `:right` is a CSS pseudo-class selector used to select all the right pages of a printed document.
- When printing double-sided documents (such as books), the pages on left and right pages may be different. The `:right` page selector is used in conjunction with the `@page` rule, which selects all pages in a printed document, to select all the right pages of the document. In other words, when used with `@page`, `:right` acts kind of like a filter used to select only the right pages.

```css
@page :right {
    /* styles for the right pages */
}
```

#### Note

- In addition to :right, a `@page` can be used in conjunction with two other pseudo-classes, namely `:first` and `:left`, which select the first page and all the left pages in double-sided documents, respectively.
- Styles specified in a `:right` `@page` rule override any styles provided in an `@page` rule that has no pseudo-class specified.
- Styles specified in a `:first` `@page` rule override any styles specified in `:left` and `:right` `@page` rules.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>