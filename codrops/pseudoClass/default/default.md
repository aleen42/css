## :default [**Back**](./../pseudoClass.md)

- `:default` is a pseudo-class selector used to select and style one or more UI elements that are the default among a set of similar elements.
- This selector typically applies to context menu items, buttons, and select lists/menus.

#### Case 1: default submit buttons

- Button inputs and buttons of type="submit" are considered one group, and therefore the first of them is the default.

```html
<input type="submit" value="Submit (<input>)">
<button type="submit">Submit (<Button>)</button>
```

```css
input[type="submit"] {
    color: #fff;
    border-radius: 4px;
    background-color: #f0f0f0;
}

input[type="submit"]:default {
    background-color: #a10000;
}

button[type="submit"] {
    color: #fff;
    border-radius: 4px;
    background-color: #f0f0f0;
}

button[type="submit"]:default {
    background-color: #a10000;
}
```

#### Case 2: default checkboxes and radio buttons

- Elements selected by `:default` also include checked checkboxes and radio buttons that have the **checked** attribute set, and options in a select menu that have the **selected** attribute set.

```html
<input type="radio" id="box-1"><label for="box-1">default radio buttons</label>
<input type="checkbox" id="box-2"><label for="box-2">default checkboxes</label>
```

```css
input[type="checkbox"]:default + label {
    text-decoration: underline;
}

input[type="checkbox"]:default + label {
    text-decoration: underline;
}
```

<p data-height="266" data-theme-id="21735" data-slug-hash="MKEejV" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/MKEejV/'>MKEejV</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>