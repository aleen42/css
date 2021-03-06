## :empty [**Back**](./../pseudoClass.md)

- `:empty` is a pseudo-class selector used to select elements in a page that are empty.
- An element counts as empty if it does not have any child elements (nodes) or text content. **Comments** and **processing instructions** do not affect whether the element is empty or not.
- Selecting empty elements is useful for hiding these elements because they may be the cause of weird(怪異的) vertical and/or horizontal white space if they have padding. It's also useful for removing empty elements in dynamic environments where empty elements are no longer needed or useful.

```html
<div><!-- comment --></div>
```

#### Note

- Generated content such as content generated by the pseudo-elements `::before` and `::after` does not count as "real" content, and therefore won't affect the emptiness of an element, even if they exist inside the element.

```css
div::after {
    content: "after content";
}

div:empty {
    background-color: #a10000;
    color: #fff;
}
```

<p data-height="266" data-theme-id="21735" data-slug-hash="GoMQOL" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/GoMQOL/'>GoMQOL</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

- Empty spaces, empty children and break-line character inside an element count as character information inside that element, and so the element is not considered empty anymore if it contains one of the three. 

```html
<!-- empty space -->
<div> </div>

<!-- empty children -->
<div></div>

<!-- break-line character -->
<div>
</div>
```

- Because white spaces are considered content, element tags that are open but not closed are also considered not empty.

```html
<p>
```

- However, if the open tag is directly followed by another tag, then it is considered empty again.

```html
<p><p>content...</p>
```

- Self-closing elements such as `<hr />`, `<br />`, and `<img />`, for example, are considered empty and will match the `:empty` selector.

<p data-height="266" data-theme-id="21735" data-slug-hash="yezvKV" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/yezvKV/'>yezvKV</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>