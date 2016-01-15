## ::first-line [**Back**](./../pseudoClass.md)

- `::first-line` is a pseudo-element used to select the first formatted line in a block-level element (such as a paragraph `<p>`).
- Like `::first-letter`, the `::first-line` pseudo-element does not select the first line of an inline-level element; that is, an element that has `display: inline`. It only works on elements that have a display value of `block`, `inline-block`, `table-cell`, `table-caption`, or `list-item`.

#### Case : select the first letter of a block quote

```html
<p>
    "Drawing from our own ignorance, and from the united ignorance of others (most freely and generously bestowed), we mapped out the details of the campaign with glibness and ease. At Vardö we were to purchase furs to wear and horses to ride."
</p>
```

```css
p::first-letter {
    font-size: 3em;
}
```

<img src="./first-letter-with-punctuation.png">

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>