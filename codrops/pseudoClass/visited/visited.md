## :visited [**Back**](./../pseudoClass.md)

- `:visited` is a pseudo-class used to select and style visited links in a page.
- Note that it will only select anchors `<a>` that have an **href** attribute.
- The `:visited` pseudo-class applies once the link has been visited by the user.

```html
<!-- will select any of these -->

<a href="#">Random Link</a>
<a href="#id">Internal Link</a>
<a href="http://codrops.com">External Link</a>

<!-- will not select this -->

<a>No href attribute</a>
```

#### Case: learning `:valid`

<p data-height="266" data-theme-id="21735" data-slug-hash="LNGPZE" data-default-tab="result" data-user="aleen42" class="codepen">See the Pen <a href="http://codepen.io/aleen42/pen/LNGPZE/">LNGPZE</a> by aleen42 (<a href="http://codepen.io/aleen42">@aleen42</a>) on <a href="http://codepen.io">CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- An element can be both `:visited` and `:active` (or `:link` and `:active`).
- When the four link styling pseudo-classes are used, they are preferably used in the following order: `:link`, `:visited`, `:hover`, and `:active`. For example:

```css
a:link {
    /** style links */
}

a:visited {
    /** style visited links */
}

a:focus {
    /** style focus state links */
}

a:hover {
    /** style hover links */
}

a:active {
    /** style active state links */
}
```

- When you're styling **links** using `:focus` it is recommended that you provide the `:focus` styles after `:link` and `:visited` styles, otherwise the `:focus` styles would be overridden by those of `:link` and `:visited`.
- The `:visited` pseudo-class can, along with some scripting, be used by websites to attack and "sniff" a user's web browsing history. In order to prevent privacy issues caused by this, modern browsers have set limitations on the kind of styles that can be applied to `:visited` links. These limitations help protect a user's privacy by preventing scripts from being able to identify and retrieve links that have been visited from a web page. The [solution to this privacy issue](http://dbaron.org/mozilla/visited-privacy) was proposed by Mozilla's David Baron.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>