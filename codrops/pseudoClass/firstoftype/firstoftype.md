## :first-of-type [**Back**](./../pseudoClass.md)

- `:first-of-type` is a pseudo-class selector that selects an element that is the first element (sibling(兄弟姐妹關係)) of its type in the list of children of its parent.

#### Case: understanding `:first-of-type`

<p data-height="266" data-theme-id="21735" data-slug-hash="OMxrLj" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/OMxrLj/'>OMxrLj</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- Differences between `:first-child` and `:first-of-type` is:

```html
<article>
    <h1>Article Title</h1>
    <p>
        First paragraph.
    </p>
    <p>
        Second paragraph.
    </p>
    <!-- .... -->
</article>
```

```css
p:first-child {
    /** styles is not applied because there is a h1 tag before the p tag */
}

p:first-of-type {
    /** stsyles will applied to the first paragrath */
}
```

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>