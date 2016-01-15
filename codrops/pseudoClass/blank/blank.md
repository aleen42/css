## :blank [**Back**](./../pseudoClass.md)

- `:blank` is a CSS pseudo-class selector used to select pages of a printed document, such as a book, that are empty as a result of a forced `page break`.

#### Case: add `:active` for anchor links and other elements

```css
a:active {
    background-color: black;
    color: white;
}

p:active {
    background-color: black;
}
```

<p data-height="266" data-theme-id="21735" data-slug-hash="rxGeNW" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/rxGeNW/'>rxGeNW</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- An element can be both `:visited` and `:active` (or `:link` and `:active`).
- When the four link styling pseudo-classes are used, they are preferably used in the following order: `:link`, `:visited`, `:hover`, and `:active`. For example:

```css
a:link {
    /** style links */
}

a:visited {
    /** style visited links */
}

a:focus {
    /** style focus state links */
}

a:hover {
    /** style hover links */
}

a:active {
    /** style active state links */
}
```

- This order is preferred because otherwise some state styles could override other state styles, thus making them not work as expected. (eg. `:visited` can override `:hover` and `active`)

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>