## :fullscreen [**Back**](./../pseudoClass.md)

- The `:fullscreen` CSS pseudo-class selector is used to select and style an element that is being displayed in **full-screen** mode.
- Most browsers have the ability to enter a **fullscreen** or **kiosk(電話亭)** mode for a while now. Basically, the browser's GUI gets out of the way, and the content takes over. In that case, the entire page is in fullscreen mode. You can see that effect by clicking `F11` while a page is active.
- For an element to match `:fullscreen`, it will have to enter **fullscreen** mode using the HTML5 [Fullscreen API](https://dvcs.w3.org/hg/fullscreen/raw-file/tip/Overview.html).
    - a simple snippet example that gets an element into fullscreen mode might look like the following:

```js
const el = document.getElementByID('element');

/** use necessary prefixed versions */
el.webkitRequestFullscreen();
el.mozRequestFullScreen();
el.msRequestFullscreen();

/** finally the standard version */
el.requestFullscreen();
```

```css
#element:fullscreen {
    width: 100vw;
    height: 100vh;
    /** etc.. */
}
```

#### Case: fullscreen to full-fill the screen

<p data-height="266" data-theme-id="21735" data-slug-hash="bEoOBM" data-default-tab="result" data-user="aleen42" class='codepen'>See the Pen <a href='http://codepen.io/aleen42/pen/bEoOBM/'>bEoOBM</a> by aleen42 (<a href='http://codepen.io/aleen42'>@aleen42</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

#### Note

- Compatibility of different browsers:

```css
#element:-webkit-fullscreen {
    width: 100vw;
    height: 100vh;
    /** etc.. */
}

#element:-moz-fullscreen {
    width: 100vw;
    height: 100vh;
    /** etc.. */
}

#element:-ms-fullscreen {
    width: 100vw;
    height: 100vh;
    /** etc.. */
}

#element:fullscreen {
    width: 100vw;
    height: 100vh;
    /** etc.. */
}
```

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>