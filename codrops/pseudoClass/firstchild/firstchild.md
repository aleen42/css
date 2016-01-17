## :first-child [**Back**](./../pseudoClass.md)

- `:first-child` is a pseudo-class which selects the target element if it is the first child of some other element.
- That is, `:first-child` will match the element only if it is the first child of its parent.

#### Case: understanding `:first-child`



#### Note

- The paragraph won't be selected as the first element in the follow case:

```html
<div class="container">
    <h1>Heading</h1>
    <p>Lorem Ipsum...</p>
</div>
```

- If you want to select and style the first paragraph inside a container, whether or not it is the first child, you can use the `:first-of-type` selector, which, as the name suggests, will select the first element of its type, whether or not it is the first child of its parent. For example, `p:first-of-type` will select the paragraph that comes after the heading in the above source code example, but will not match any other paragraph that comes after that.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>