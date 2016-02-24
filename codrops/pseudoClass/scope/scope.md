## :scope [**Back**](./../pseudoClass.md)

- The `:scope` CSS pseudo-class selector represents any element that is a `:scope` element.
- A **scope element** is an element that forms a context for a block of styles. Such an element also provides a reference point for selectors to match against.
- A scope element can be defined using the scoped attribute. A simple example would look like the following:

```html
<section>
    <style scoped>
        /* style declarations here apply to the <section>'s content */
        p {
            color: #0099cc; /* a blue color */
        }
    </style>
    <p>
        I am in the scope.
    </p>
</section>
<p>
    I am outside the scope.
</p>
```

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>