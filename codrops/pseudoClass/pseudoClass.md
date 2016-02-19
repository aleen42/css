## Pseudo [**Back**](./../codrops.md)

#### Pseudo Elements

- [**::after**](./after/after.md)
- [**::before**](./before/before.md)
- [**::first-letter**](./firstletter/firstletter.md)
- [**::first-line**](./firstline/firstline.md)
- [**::placeholder**](./placeholder/placeholder.md)
- [**::selection**](./selection/selection.md)

#### Pseudo Classes

- [**:active**](./active/active.md)
- [**:blank**](./blank/blank.md)
- [**:check**](./check/check.md)
- [**:default**](./default/default.md)
- [**:dir()**](./dir/dir.md)
- [**:disabled**](./disabled/disabled.md)
- [**:empty**](./empty/empty.md)
- [**:enabled**](./enable/enable.md)
- [**:first**](./first/first.md)
- [**:first-child**](./firstchild/firstchild.md)
- [**:first-of-type**](./firstoftype/firstoftype.md)
- [**:focus**](./focus/focus.md)
- [**:fullscreen**](./fullscreen/fullscreen.md)
- [**:hover**](./hover/hover.md)
- [**:in-range**](./inrange/inrange.md)
- [**:indeterminate**](./indeterminate/indeterminate.md)
- [**:invalid**](./invalid/invalid.md)
- [**:lang()**](./lang/lang.md)
- [**:last-child**](./lastchild/lastchild.md)
- [**:last-of-type**](./lastoftype/lastoftype.md)
- [**:left**](./left/left.md)
- [**:link**](./link/link.md)
- [**:not()**](./not/not.md)
- [**:nth-child()**](./nthchild/nthchild.md)
- [**:nth-last-child()**](./nthlastchild/nthlastchild.md)
- [**:nth-of-type()**](./nthoftype/nthoftype.md)
- [**:nth-last-of-type()**](./nthlastoftype/nthlastoftype.md)
- [**:only-child**](./onlychild/onlychild.md)
- [**:only-of-type**](./onlyoftype/onlyoftype.md)
- [**:optional**](./optional/optional.md)
- [**:out-of-range**](./outofrange/outofrange.md)
- [**:read-only**](./readonly/readonly.md)
- [**:read-write**](./readwrite/readwrite.md)
- [**:required**](./required/required.md)
- [**:required**](./required/required.md)

#### Note

###### Different notations: (`:`) and (`::`)

- In CSS1 and CSS2, pseudo-elements were defined to start with one colon (`:`), just like pseudo-classes (for example `:hover`). To distinguish pseudo-elements from pseudo-classes, the double colon notation (`::`) is used in CSS3. (*`:` for pseudo classes, `::` for pseudo elements*)
- All browsers that support the two-colon notation also support the one-colon notation. **Internet Explorer 8**, however, does not support the two-colon notation. So, unless you need to support Internet Explorer 8, you can use the two-colon notation without having to worry about browser support.
- It's recommended that using `::` to distinguish them.

```css
/**
 * bad
 */
.example:after {
    /** css */
}

/**
 * good
 */
.example::after {
    /** css */
}
```

###### About accessability

- Content added using pseudo-elements is not inserted into the DOM—it is only visually displayed. Hence, screen readers won’t be able to access and read the content generated using pseudo-elements. So, it is recommended that you don’t use pseudo-elements to insert vital content into a page (such as footer notes that are relevant to the article, for example).
- Pseudo-elements are mostly used to insert and style cosmetic content, and should not be relied on to insert content that is relevant to the meaning and completeness of the content on the page.
- Also, since the content inserted using pseudo-elements is not inserted into the DOM, this means that you cannot attach any event handlers to it using JavaScript.

###### About IE compatibility

- Internet Explorer does not support using z-index on pseudo-elements.
- The two-colon syntax introduced in CSS Level 3 is not supported in **Internet Explorer 8** and earlier, only the single-colon syntax is supported in those versions down to version 5.5.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../pic/tail.gif"></a>