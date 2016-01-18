## :invalid [**Back**](./../pseudoClass.md)

- `:invalid` is a CSS pseudo-class used to select and style form `<input>` elements whose value is invalid according to its type specified in the **type** attribute.
- For example, number input types (`<input type="number">`) that have an alphabet character value, or email inputs (`<input type="email">`) whose value does not match a valid email address pattern.
- In some browsers, :invalid also matches a form (`<form>`) and a fieldset (`<fieldset>`) that have one or more input elements that have invalid values according to their type value.

#### Case: learning `:invalid`

<p data-height="266" data-theme-id="21735" data-slug-hash="ZQazoL" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/ZQazoL/'>ZQazoL</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- When a number input type (`<input type="number">`) is out of the range of permitted values specified using the **min** and **max** attributes, then the `:invalid` pseudo-class matches, and also the `:out-of-range` pseudo-class matches. Any styles applied using `:out-of-range` will override the styles applied using `:invalid`. 
- The `:invalid` pseudo-class also applied to all of the buttons in a group of radio buttons (they have the same name attribute value) if one of the buttons is required (has the required attribute) but none of the buttons in the group is selected.
- Using `:invalid` to select a form that has an invalid input currently only works in **Firefox 13+**.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>