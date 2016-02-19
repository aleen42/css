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
- According to rules `@page`, you can only change some CSS properties:

categories|items
----------|-----
**Margin Properties**|`margin-top`, `margin-left`, `margin-right`, and `margin-bottom`
**Page Break Properties**|`page-break-after`, `page-break-before`, and `page-break-inside`
**Other Properties**|`orphans` and `windows`

- All pages are automatically classified by user agents into either the `:left` or `:right` pseudo-class. Whether the first page of a document is `:left` or `:right` depends on the major writing direction of the root element. For example, the first page of a document with a **left-to-right** major writing direction would be a `:right` page, and the first page of a document with a **right-to-left** major writing direction would be a `:left` page. To explicitly force a document to begin printing on a left or right page, authors can insert a **page break** before the first generated box.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>