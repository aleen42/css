## ::before [**Back**](./../pseudoClass.md)

- The content inserted using `::before` is inserted before other content inside the element and is displayed inline by default. The value of the content is specified using the [`content`]() property.
- Case: **add a small icon to all links**

```html
Let's <a href="#" class="external">Move The Web Forward</a> together!
```

```css
.external::after {
    content: url(external-link.png);
    padding-left: 5px;  /** create some space between the icon and the link */
}
```

<img src="./inspecting-after.png">

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>