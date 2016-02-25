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
- So, in more technical words: the `:target` pseudo-class selects the unique element, if any, with an ID matching the fragment identifier of the URI of the document.

#### The Yellow Fade Technique - Highlighting The Target Element

- The Yellow Fade Technique(YFT) was [introduced by 37 Signals](http://signalvnoise.com/archives/000558.php) to highlight newly added content in a page in order to attract the user's attention to it.
- Using the same principle of highlighting content to attract a user's attention or **guide a user's eye**, the `:target` pseudo-class can be very useful for highlighting target elements inside a page when the browser scrolls (or jumps) to those elements. But why would you want to (or need to) do that? The browser would normally scroll down to the target element enough so that the element sticks at the top of the viewport, thus bringing attention to that element. But what if the browser can't scroll down enough to do that because there isn't enough vertical space to allow that amount of scrolling? For example, if the target element is at the end of the page with no enough content after it to allow more scrolling, the browser won't be able to stick it at the top of the viewport. In this case, clicking the link will scroll the page down to the element but it won't be clear which element is the target element because it won't be the one stuck at the top of the viewport.
- This is where the `:target` pseudo-class comes in use. Using `:target`, we can recreate the YFT with CSS3 animations to highlight the target element to attract the reader's eye to it so that she knows that it is the target of the link she clicked.

#### Case: learning `:target`

- To better understand that, click on any of the links on the left in the following demo. Each link targets a corresponding section. When you click on a link, its corresponding section is scrolled to the top of the viewport. But when you click on the last section, the browser will scroll down enough so that the section is in the viewport, but it can't scroll down more to stick the last section to the top of the viewport since there isn't enough content after it to allow that.


<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>