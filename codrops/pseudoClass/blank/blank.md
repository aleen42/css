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
- Also, styles specified in a `:blank` `@page` rule override any styles provided in `:left` and `:right` `@page` rules. (`:left` and `:right` are selectors used to select the left pages and the right pages of a double-sided printed document, such as a book.)
- The `page-break-before` and `page-break-after` properties will be replaced with `break-before` and `break-after` properties, respectively, in a future CSS level.
- According to rules `@page`, you can only change some CSS properties:

categories|items
----------|-----
**Margin Properties**|`margin-top`, `margin-left`, `margin-right`, and `margin-bottom`
**Page Break Properties**|`page-break-after`, `page-break-before`, and `page-break-inside`
**Other Properties**|`orphans` and `windows`

###### at-rules

- In CSS3, at-rules that select and target page margins were introduced. They have **no browser support** at this time. But the following is an example of how you might style an empty page using a page margin at-rule; the example inserts content into the center of the top margin of an empty page:


<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>