## Pseudo [**Back**](./../codrops.md)

#### Pseudo Classes

- [**::after**](./after/after.md)
- [**::before**](./before/before.md)

#### Note

###### Different notations: (`:`) and (`::`)

- In CSS1 and CSS2, pseudo-elements were defined to start with one colon (`:`), just like pseudo-classes (for example [`:hover`]()). To distinguish pseudo-elements from pseudo-classes, the double colon notation (`::`) is used in CSS3. (*`:` for pseudo elements, `::` for pseudo classes*)
- All browsers that support the two-colon notation also support the one-colon notation. **Internet Explorer 8**, however, does not support the two-colon notation. So, unless you need to support Internet Explorer 8, you can use the two-colon notation without having to worry about browser support.
- It's recommended that using `::` to distinguish them.

```css
/**
 * bad
 */
.example:after {
    /** css */
}

/**
 * good
 */
.example::after {
    /** css */
}
```

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../pic/tail.gif"></a>