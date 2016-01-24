## :link [**Back**](./../pseudoClass.md)

- `:link` is a pseudo-class used to select and style links in a page. It is important to note, though, that it will only select links `<a>` that have an **href** attribute.

```html
<!-- will select any of these -->

<a href="#">Random Link</a>
<a href="#id">Internal Link</a>
<a href="http://codrops.com">External Link</a>

<!-- will not select this -->

<a>No href attribute</a>
```

#### Case: Learning `:link`



#### Note

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

- The `:link` pseudo-class will select all links, even those that are already styled using any of the other three pseudo-classes. So, the styles applied using `:visited` will be overridden by the styles applied using `:link`.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>