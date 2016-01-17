## :focus [**Back**](./../pseudoClass.md)

- `:focus` is a pseudo-class used to select and style elements, usually **links** and **form** elements, that have been focused by the user, either by "tabbing" using the keyboard or by clicking.
- Form elements, such as `<input>`, `<button>`, and `<textarea>` can receive focus either by tabbing using the keyboard or by clicking. An input field or a textarea are in focus when they are clicked and ready to be typed in.
- When the user tabs through links and form elements in a page, the browser usually adds a dotted outline around the element that is currently receiving the tab focus. The styles added by the browser are default to each browser and usually don't look the same across browsers, so you may want to override the default styles and replace them with your own.
- The browser uses the `outline` CSS property in its default style sheet to add the `:focus` styles to focused elements.

```html
<input type="text" name="searchBar" value="">
```

```css
input[type="text"]:focus {
    outline: none;  /* disabled the default property, 
                     * and of course you can change it like 
                     * outline: 1px solid #a10000;
                     */
                     
    /** add your own styles down here */
    border: 1px solid #a10000;
}
```

<p data-height="266" data-theme-id="21735" data-slug-hash="jWGXPp" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/jWGXPp/'>jWGXPp</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- When you're styling **links** using `:focus` it is recommended that you provide the `:focus` styles after `:link` and `:visited` styles, otherwise the `:focus` styles would be overridden by those of `:link` and `:visited`.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>