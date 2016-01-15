## ::first-line [**Back**](./../pseudoClass.md)

- `::first-line` is a pseudo-element used to select the first formatted line in a block-level element (such as a paragraph `<p>`).

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