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
- According to rules `@page`, you can only change some CSS properties:

categories|items
----------|-----
**Margin Properties**|`margin-top`, `margin-left`, `margin-right`, and `margin-bottom`
**Page Break Properties**|`page-break-after`, `page-break-before`, and `page-break-inside`
**Other Properties**|`orphans` and `windows`

- All pages are automatically classified by user agents into either the `:left` or `:right` pseudo-class. Whether the first page of a document is `:left` or `:right` depends on the major writing direction of the root element. For example, the first page of a document with a **left-to-right** major writing direction would be a `:right` page, and the first page of a document with a **right-to-left** major writing direction would be a `:left` page.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>