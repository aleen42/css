## :dir() [**Back**](./../pseudoClass.md)

- `:dir()` CSS pseudo-class selector is used to select an element based on its directionality as determined by the document language.
- The direction of text in an element can be specified using the CSS `direction` property. However, the `:dir()` pseudo-class selector does not match an element whose directionality is solely(僅) specified using the direction property. The directionality needs to be specified in the document to match the selector, not in CSS, because `:dir()` does not select based on stylistic states.
- In an HTML5 document, the directionality of an element can be specified using the dir attribute. The directionality can be set to either **ltr**(left-to-right) or **rtl**(right-to-left) (If a future markup specification defines other directionalities, then CSS Selectors may be extended to allow corresponding values). For example:

```html
<article dir="rtl">
    <!-- ... -->
</article>
```

#### Note

- The usage of `:dir()` is not equivalent to the usage of the `[dir = ""]` selector.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>