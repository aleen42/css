## ::first-letter [**Back**](./../pseudoClass.md)

- `::first-letter` is a pseudo-element which selects the first letter in the first line of a block-level element (such as a paragraph `<p>`), if that letter is not preceded by any other content (such as **images** or **inline tables**) on its line.
- The `::first-letter` pseudo-element does not select the first letter of an inline-level element; that is, an element that has `display: inline`. It only works on elements that have a display value of `block`, `inline-block`, `table-cell`, `table-caption`, or `list-item`.
- Notice that: **Punctuation(標點符號)** (i.e, characters defined in Unicode in the "open" (Ps), "close" (Pe), "initial" (Pi). "final" (Pf) and "other" (Po) punctuation classes), that precedes or follows the first letter should be included in `::first-letter`.

#### Case : add a quote before a block quote

```html
<blockquote>
    Your present circumstances don't determine where you can go; they merely determine where you start.—Nido Qubein
</blockquote>
```

```css
blockquote::before {
    content: "\201C"; /** style of the quote */
    color: deepPink;
    font-size: 3em;
    position: relative;
    top: 20px;
}
```

<img src="./inspecting-before.png">

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>