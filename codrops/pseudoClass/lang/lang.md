## :lang() [**Back**](./../pseudoClass.md)

- `:lang()` is a CSS pseudo-class selector that matches an element based on the language it is determined to be in.
- A language is determined in HTML using a combination of the **lang** attribute (e.g `<html lang="en">`), the `<meta>` tag, and possibly by information from the protocol (such as **HTTP headers**). **XML** uses an attribute called `xml:lang`, and there may be other document language-specific methods for determining the language.

```css
.element:lang(X) {
    /** styles for the element which is in the language X */
    /*
     * Whether an element is represented by a :lang() selector is based solely on 
     * the element’s language value being equal to the identifier X,
     * or beginning with the identifier X immediately followed by "-" (U+002D).
     */
}
```


<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>