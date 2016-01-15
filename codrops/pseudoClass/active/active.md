## :active [**Back**](./../pseudoClass.md)

- `:active` is a CSS pseudo-class. It specifies and selects an element based on a state, the active state, and is used to apply styles to an element when it matches that state.
- The `:active` pseudo-class is a dynamic class which applies when an element is being activated by the user. It is often used to target and style an element when it's **active** (as the name suggests). More specifically, it targets an element (usually an anchor link `<a>`) between the time it is clicked on and the time it is released.

#### Case: add :active for anchor links and other elements

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


<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>