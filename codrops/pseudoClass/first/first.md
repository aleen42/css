## :first [**Back**](./../pseudoClass.md)

- `:first` is a CSS pseudo-class selector used to select the first page of a printed document.
- It is used in conjunction with the `@page` rule which selects all pages in a printed document. So, when used with `@page`, `:first` acts kind of like a filter used to select only the first page among all pages.

```css
@page :first {
    /** styles for the first page */
}
```

#### Case: distinguished first page

```css
/* All margins set to 2cm */
@page { 
    margin: 2cm;
} 

/* Top margin on first page 10cm */
@page :first {
    margin-top: 10cm;    
}
```

#### Note

- In addition to `:first`, a `@page` can be used in conjunction with two other pseudo-classes, namely `:left` and `:right`, which select the left and right pages in double-sided documents, respectively.
- Styles specified in a `:first` `@page` rule override any styles specified in `:left` and `:right` `@page` rules.
- According to rules `@page`, you can only change some CSS properties:

categories|items
----------|-----
**Margin Properties**|`margin-top`, `margin-left`, `margin-right`, and `margin-bottom`
**Page Break Properties**|`page-break-after`, `page-break-before`, and `page-break-inside`
**Other Properties**|`orphans` and `windows`

- All pages are automatically classified by user agents into either the `:left` or `:right` pseudo-class. Whether the first page of a document is `:left` or `:right` depends on the major writing direction of the root element. For example, the first page of a document with a **left-to-right** major writing direction would be a `:right` page, and the first page of a document with a **right-to-left** major writing direction would be a `:left` page.
- If a forced break occurs before the first generated box, it is undefined in CSS 2.1 whether `:first` applies to the blank page before the break or to the page after it.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>