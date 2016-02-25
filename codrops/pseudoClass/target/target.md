## :target [**Back**](./../pseudoClass.md)

- The `:target` pseudo-class is used to style an element that is the target of an internal link in a document.
- Some web pages contain links that point to certain sections or elements on the same page, instead of pointing to other pages. Such links point to elements in the page that have a certain ID, and they point to them by using an element's ID as the value for the link's href attribute. For example, the following link points to an element on the page with an ID of **article-demo**.

```html
<a href="#artical-demo">Go To Demo</a>

<!-- somewhere in the page an element with an ID "article-demo" exists -->
<section id="article-demo">
    <!-- content here -->
</section>
```

- When the link is clicked, the URI of the page gets what is known as a fragment identifier, which **identifies** the element in the page which is **the target** that the link points to. URIs with fragment identifiers at the end link to a certain element in the document, known as the target element. **The `:target` pseudo-class is used to style that element.**

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>