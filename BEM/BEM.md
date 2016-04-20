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
div.block__elem { color: #042; }
```

#### Modifier

Modifier names may consist of Latin letters, digits, dashes and underscores. CSS class is formed as block’s or element’s name plus two dashes: .block--mod or .block__elem--mod and .block--color-black with .block--color-red. Spaces in complicated modifiers are replaced by dash.

- <a href="http://aleen42.github.io/" target="_blank" ><img src="./../pic/tail.gif"></a>