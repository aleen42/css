## Font Content with Values [**Back**](./../README.md)

- There is a list of Font Awesome icons and their CSS content values:
- [Font Awesome](http://fortawesome.github.com/Font-Awesome/) is a web font containing all the icons from the Twitter Bootstrap framework, and now many more. Whilst the implementation in Bootstrap is designed to be used with the `<i>` element (Bootstrap v2), you may find yourself wanting to use these icons on other elements. To do so, you'll need to use the following CSS on the desired element, and then substitute in the content value for the relevant icon.

```css
.element {
    position: relative;
}
 
/**
 * replace the content value with the
 * corresponding value from the list below
 */
 
.element:before {
    content: "\f000";
    font-family: FontAwesome;
    font-style: normal;
    font-weight: normal;
    text-decoration: inherit;

    /** adjust as necessary */
    color: #000;
    font-size: 18px;
    padding-right: 0.5em;
    position: absolute;
    top: 10px;
    left: 0;
}
```

#### Useage

- the first thing you should do is to load font of Font Awesome from the follow fonts(download them and put them in an directory like `fonts/`):
    - [FontAwesome.otf](https://github.com/aleen42/css/blob/master/content/fonts/FontAwesome.otf?raw=true)
    - [fontawesome-webfont.eot](https://github.com/aleen42/css/blob/master/content/fonts/fontawesome-webfont.eot?raw=true)
    - [fontawesome-webfont.svg](https://github.com/aleen42/css/raw/master/content/fonts/fontawesome-webfont.svg?raw=true)
    - [fontawesome-webfont.ttf](https://github.com/aleen42/css/blob/master/content/fonts/fontawesome-webfont.ttf?raw=true)
    - [fontawesome-webfont.woff](https://github.com/aleen42/css/blob/master/content/fonts/fontawesome-webfont.woff?raw=true)
    - [fontawesome-webfont.woff2](https://github.com/aleen42/css/blob/master/content/fonts/fontawesome-webfont.woff2?raw=true)

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../pic/tail.gif"></a>