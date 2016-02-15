## :nth-child() [**Back**](./../pseudoClass.md)

- The `:nth-child()` is a CSS pseudo-class selector that allows you to select elements based on their index (source order) inside their container.
- You can pass in a **positive number** as an argument to `:nth-child()`, which will select the one element whose index inside its parent matches the argument of `:nth-child()`. For example, `li:nth-child(3)` will select the list item with an index value **3**; that is, it will select the third list item.
- You can also pass in one of two predefined keywords: **even** and **odd**.
    - `li:nth-child(even)` will select all list items with even index numbers **(2, 4, 6, 8, etc.)**
    - `li:nth-child(odd)` will select all list items with odd index numbers **(1, 3, 5, 7, etc.)**
- You can also use a **formula** (or an **equation**)
    - `li:nth-child(an+b)`: to divide into **a** groups and select the **b**th element of each group.

#### Note

- Using some tools to help dealing with the calculations for `nth-child` by visualizing.
    - [CSS3 structural pseudo-class selector tester](http://lea.verou.me/demos/nth.html) by *Lea Verou*
    - [NTH-TEST – nth-child and nth-of-type tester](http://nth-test.com/) by *Paul Maloney*

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a