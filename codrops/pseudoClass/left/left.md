## :left [**Back**](./../pseudoClass.md)

- `:left` is a CSS pseudo-class selector used to select all the left pages of a printed document.
- When printing double-sided documents (such as books), the pages on left and right pages may be different. The `:left` page selector is used in conjunction with the `@page` rule, which selects all pages in a printed document, to select all the left pages of the document.

```css
@page :left {
    /** styles for left pages */
}
```

#### Note:

- Styles specified in a `:first` `@page` rule override any styles specified in `:left` and `:right` `@page` rules.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>