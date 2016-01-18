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

#### Case: Learning `:lang()`

<p data-height="266" data-theme-id="21735" data-slug-hash="gPXYZN" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/gPXYZN/'>gPXYZN</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- A language is usually specified on the root **html** element and is therefore inherited by the information in the **head** and the **body**, but it can also be specified on any element in the page.

```html
<p>You'd say that in Chinese as <span lang="zh-Hans">中國科學院文獻情報中心</span></p>
```

- Language codes consist of a primary code and a possibly empty series of subcodes: `language-code = primary-code ( "-" subcode )*`. Example language codes include "en" for English, "zh-Hans" for Chinese, and "en-GB-oed" for English based on the Oxford English Dictionary spelling. In order to choose the right language code, you can check the list of available language codes out in the [**IANA** language sub-tag registry](http://www.iana.org/assignments/language-subtag-registry/language-subtag-registry).

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>