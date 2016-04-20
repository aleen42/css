## BEM Naming [**Back**](./../README.md)

> There are only two hard problems in Computer Science: cache invalidation and naming things — Phil Karlton

#### Block

Block names may consist of Latin letters, digits, and dashes. To form a CSS class, add a short prefix for namespacing: `.block`.

```html
<div class="block">...</div>
```

```css
.block { color: #042; }
```

#### Element

Element names may consist of Latin letters, digits, dashes and underscores. CSS class is formed as block name plus two underscores plus element name: `.block__elem`

```html
<div class="block">
    ...
    <span class="block__elem"></span>
</div>
```

```css
/** good */
.block__elem { color: #042; }

/** bad */
.block .block__elem { color: #042; }
```

- <a href="http://aleen42.github.io/" target="_blank" ><img src="./../pic/tail.gif"></a>