## :only-child [**Back**](./../pseudoClass.md)

- `:only-child` is a CSS pseudo-selector which matches an element if it is its parent's only child. That is, the element is selected only if its parent has no other children of any type.
- For example, `li:only-child` will match a list item only if it is the only item in the list. `p:only-child` will match a paragraph only if it is the only child inside its container. So, it will select the following paragraph:

```html
<article>
    <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Soluta, enim, libero voluptatum id nostrum porro laborum error nisi fugit atque a possimus ullam maxime quia tenetur obcaecati dolorum dolore placeat.
    </p>
</article>
```
- But it will not match the following paragraph, since it is not the only child of its parent:

```html
<article>
    <h1>Heading</h1>
    <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus, iusto, eos similique eaque minus magni tempore repudiandae mollitia dignissimos obcaecati animi quis et impedit consectetur optio modi perferendis voluptate corporis!
    </p>
</article>
```


<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>