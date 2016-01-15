## ::first-letter [**Back**](./../pseudoClass.md)

- `::first-letter` is a pseudo-element which selects the first letter in the first line of a block-level element (such as a paragraph `<p>`), if that letter is not preceded by any other content (such as images or inline tables) on its line.
- The content inserted using `::before` is inserted before other content inside the element and is displayed inline by default. The value of the content is specified using the [`content`]() property.

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