## ::first-letter [**Back**](./../pseudoClass.md)

- `::first-letter` is a pseudo-element which selects the first letter in the first line of a block-level element (such as a paragraph `<p>`), if that letter is not preceded by any other content (such as **images** or **inline tables**) on its line.
- The `::first-letter` pseudo-element does not select the first letter of an inline-level element; that is, an element that has `display: inline`. It only works on elements that have a display value of `block`, `inline-block`, `table-cell`, `table-caption`, or `list-item`.
- Notice that: **Punctuation(標點符號)** (i.e, characters defined in Unicode in the "open" (Ps), "close" (Pe), "initial" (Pi). "final" (Pf) and "other" (Po) punctuation classes), that precedes or follows the first letter should be included in `::first-letter`.

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

<p data-height="266" data-theme-id="21735" data-slug-hash="vLeNgO" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/vLeNgO/'>vLeNgO</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- Only a subset of properties can be used to `::first-letter`:

categories|items
----------|-----
**Font Properties**|`font`, `font-style`, `font-variant`, `font-weight`, `font-size`, `line-height`, and `font-family`. `text-decoration`, `text-transform`, `letter-spacing`, `word-spacing` (when appropriate), `float`, `vertical-align` (only if `float` is none), and `color`.
**Margin Properties**|`margin`, `margin-top`, `margin-right`, `margin-bottom`, and `margin-left`.
**Padding Properties**|`padding`, `padding-top`, `padding-right`, `padding-bottom`, and `padding-left`
**Border Properties**|`border`, `border-width`, `border-style`, `border-color`, and the corresponding longhand properties for each of these properties.
**Background Properties**|`background`, `background-color`, `background-image`, `background-position`, `background-repeat`, `background-size`, and `background-attachment`.

- If an element is a list item (`display: list-item`), the `:first-letter` applies to the first letter in the principal box after the `marker`. User agents may ignore `:first-letter` on list items with `list-style-position: inside`.
- The first letter of a `table-cell` or `inline-block` cannot be the first letter of an ancestor element. For example, in the following markup (*the first letter of the div is not the letter “H”. In fact, the div does not have a first letter.*):

```html
<div>
    <p style="display: inline-block">
        Hello
        <br>
        Goodbye
    </p> 
    etcetera
</div>
```



<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>