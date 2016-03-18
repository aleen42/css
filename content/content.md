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
 
.element::efore {
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
- then, load them into css:

```css
/*  Font Awesome
    the iconic font designed for use with Twitter Bootstrap
    -------------------------------------------------------
    The full suite of pictographic icons, examples, and documentation
    can be found at: http://fortawesome.github.com/Font-Awesome/

    License
    -------------------------------------------------------
    The Font Awesome webfont, CSS, and LESS files are licensed under CC BY 3.0:
    http://creativecommons.org/licenses/by/3.0/ A mention of
    'Font Awesome - http://fortawesome.github.com/Font-Awesome' in human-readable
    source code is considered acceptable attribution (most common on the web).
    If human readable source code is not available to the end user, a mention in
    an 'About' or 'Credits' screen is considered acceptable (most common in desktop
    or mobile software).

    Contact
    -------------------------------------------------------
    Email: dave@davegandy.com
    Twitter: http://twitter.com/fortaweso_me
    Work: Lead Product Designer @ http://kyruus.com

    */

@fontAwesomePath: '../fonts';
@font-face {
    font-family: 'FontAwesome';
    src: url('./../fonts/fontawesome-webfont.eot');
    src: url('./../fonts/fontawesome-webfont.eot?#iefix') format('embedded-opentype'), url('./../fonts/fontawesome-webfont.woff') format('woff'), url('./../fonts/fontawesome-webfont.ttf') format('truetype'), url('./../fonts/fontawesome-webfont.svg#FontAwesome') format('svg');
    font-weight: normal;
    font-style: normal;
}
```

- so you can use them like this:

```css
.element::before {
    content: "\f000";
    font-family: FontAwesome;
}
```

- <a href="http://aleen42.github.io/" target="_blank" ><img src="./../pic/tail.gif"></a>