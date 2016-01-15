## :active [**Back**](./../pseudoClass.md)

- `:active` is a CSS pseudo-class. It specifies and selects an element based on a state, the active state, and is used to apply styles to an element when it matches that state.
- The `:active` pseudo-class is a dynamic class which applies when an element is being activated by the user. It is often used to target and style an element when it's **active** (as the name suggests). More specifically, it targets an element (usually an anchor link `<a>`) between the time it is clicked on and the time it is released.

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