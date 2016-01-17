## :hover [**Back**](./../pseudoClass.md)

- `:hover` is a pseudo-class used to select and style an element when it is being hovered by the user.
- An element is hovered over when the user designates it with a pointing device, like pointing at it by placing the mouse over it, without necessarily **activating** it.
- `:hover` is a dynamic pseudo-class that matches when an element is being hovered by the user. It is usually used to give users visual feedback that the element they're pointing at has been indeed hovered and may be activated.

#### Case 1: hover actions for links

```html
<a href="#">links</a>
```

```css
a:hover {
    background-color: #a10000;
    color: #fff;
}
```

#### case 2: dropdown menu



<p data-height="266" data-theme-id="21735" data-slug-hash="rxGoGB" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/rxGoGB/'>rxGoGB</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- Most **touch devices** don't support hover interactions. Using `:hover` on touch devices can cause problems like unexpected effects and interactions.
- It is recommended that suitable fallback is provided for **touch devices** to make sure that all content is available for users on devices that don't offer `:hover` interactions.
- The `:hover` styles may be overridden by `link`, `visited`, and `focus` when applying styles.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>