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


<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>