## :default [**Back**](./../pseudoClass.md)

- `:default` is a pseudo-class selector used to select and style one or more UI elements that are the default among a set of similar elements.
- This selector typically applies to context menu items, buttons, and select lists/menus.
- Elements selected by `:default` also include checked checkboxes and radio buttons that have the **checked** attribute set, and options in a select menu that have the **selected** attribute set. 

#### Case 1: default submit buttons

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

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>