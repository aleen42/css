## :nth-of-type() [**Back**](./../pseudoClass.md)

- The `:nth-of-type()` is a CSS pseudo-class selector that allows you to select **elements of the same type** based on their index (source order) inside their container.
- You can also pass **positive number**, **predefined keywords(even, odd)** and **formula** to `nth-of-tpye()` like `nth-last-child()`.

#### Case: learning `:nth-last-of-type()`

<p data-height="266" data-theme-id="21735" data-slug-hash="BjbNmx" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/BjbNmx/'>BjbNmx</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- Using some tools to help dealing with the calculations for `nth-child` by visualizing.
    - [CSS3 structural pseudo-class selector tester](http://lea.verou.me/demos/nth.html) by *Lea Verou*
    - [NTH-TEST – nth-child and nth-of-type tester](http://nth-test.com/) by *Paul Maloney*
- There is a pseudo-class selector that has a similar functionality to that of `:nth-of-type()`, that selector is the `:nth-last-of-type()` selector. `:nth-last-of-type()` is similar to `:nth-of-type()`, except that instead of iterating through the elements from the first one downwards, it starts iterating from the last element up.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>