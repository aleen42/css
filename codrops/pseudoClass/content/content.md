## content [**Back**](./../pseudoClass.md)

- The `content` property is used with the `::before` and `::after` pseudo-elements to generate content that is to be inserted into an element in the page.
- The content inserted using the content property can be string(s) of text, glyphs, images, counters (for styling lists), or quotes. Combining multiple values into one is also possible.

```css
content: normal | none | [ <string> | <uri> | <counter> | attr(<identifier>) | open-quote | close-quote | no-open-quote | no-close-quote ]+ | inherit
```

#### Note

- The content property must be included in the set of rules for the `::before` and `::after` pseudo-elements, otherwise they won't be generated and inserted. 
- Content inserted into a page using pseudo-elements is not inserted into the DOM - it is only visually displayed. Hence, screen readers won't be able to access and read the content generated using pseudo-elements. So, it is recommended that you don't use pseudo-elements to insert vital content into a page.
- Also, since the content inserted using pseudo-elements is not inserted into the DOM, this means that you cannot attach any event handlers to it using JavaScript.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>