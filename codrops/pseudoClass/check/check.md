## :check [**Back**](./../pseudoClass.md)

- Radio (`<input type="radio">`) and checkbox (`<input type="checkbox">`) elements can be toggled by the user. Some menu items are "checked" when the user selects them. When such elements are toggled "on" the `:checked` pseudo-class applies.
- `:checked` is used to select and style checkbox (`<input type="checkbox">`), radio (`<input type="radio">`) or option (`<option></option>` in a `<select></select>`) that are checked or toggled "on" by the user.

#### Case: check the checkbox and radio

```html
<input type="radio" id="box-1" checked><label for="box-1">radio</label>
<input type="checkbox" id="box-2" checked><label for="box-2">checkbox</label>
```

<p data-height="266" data-theme-id="21735" data-slug-hash="OMxNrV" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/OMxNrV/'>OMxNrV</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Case: selected option

```html
<select name="options" id="list">
    <option value="Something" selected>This option is selected</option>
    <option value="Something-else">This one is not</option>
</select>
```

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>