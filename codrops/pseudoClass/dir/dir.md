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

```css
artical[dir="rtl"] {
    /** styles applied to article elements that have a rtl directionality set using the dir attribute */
}

artical:dir(rtl) {
    /** styles applied to artical elements that have a rtl directionality event if it's inherited */
}
```

- The usage of `:dir()` is not equivalent to the usage of the `[dir = ""]` selector.
- The `[dir = ""]` attribute selector only performs a comparison against a given attribute on the element. This means that it will match an element only if it has the dir attribute set.Moreover, if the dir attribute has a value `auto`, it will match **neither** `[dir = "ltr"]` **nor** `[dir = "rtl"]`.
- The `:dir()` pseudo-class selector, on the other hand, will match an element even if its directionality is inherited from its closest ancestor with a valid dir attribute. Also, an element that matches that has `dir="auto"` will match either `:dir(ltr)` or `:dir(rtl)` depending on the resolved directionality of the elements as determined by its contents.
- It's currently only supported by Firefox browser, and see the examples with Firefox to clarify the differences between `[dir=""]` and `:dir()`. (`[dir=""]` is supported by Chrome at this time, but not `:dir()`)

###### [dir=""]

<p data-height="266" data-theme-id="21735" data-slug-hash="adLBZL" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/adLBZL/'>adLBZL</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

###### :dir()

<p data-height="266" data-theme-id="21735" data-slug-hash="PZJbzg" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/PZJbzg/'>PZJbzg</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>