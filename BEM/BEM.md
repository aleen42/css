## BEM Naming [**Back**](./../README.md)

> There are only two hard problems in Computer Science: cache invalidation and naming things — Phil Karlton

**BEM** is a highly useful, powerful and simple naming convention to make your front-end code easier to read and understand, easier to work with, easier to scale, more robust and explicit and a lot more strict.

#### Block

**Block**: Encapsulates a standalone entity that is meaningful on its own. While blocks can be nested and interact with each other, semantically they remain equal; there is no precedence or hierarchy. Holistic entities without DOM representation (such as controllers or models) can be blocks as well.

Block names may consist of Latin letters, digits, and dashes. To form a CSS class, add a short prefix for namespacing: `.block`.

```html
<div class="block">...</div>
```

```css
.block { color: #042; }
```

#### Element

**Element**: Parts of a block and have no standalone meaning. Any element is semantically tied to its block.

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

**Modifer**: Flags on blocks or elements. Use them to change appearance, behavior or state.

Modifier names may consist of Latin letters, digits, dashes and underscores. CSS class is formed as block's or element's name plus two dashes: `.block--mod` or `.block__elem--mod` and `.block--color-black` with `.block--color-red`. Spaces in complicated modifiers are replaced by dash.

```html
<!-- good -->
<div class="block block--mod">...</div>
<div class="block block--size-big block--shadow-yes">...</div>

<!-- bad -->
<div class="block--mod">...</div>
```

```css
/** use modifier class name as selector */
.block--hidden { opacity: 0; }

/** alert elements based on a block-level modifier */
.block--mod .block__elem { text-align: center; }

/** element modifier */
.block__elem--mod { }
```

#### Example

```html
<form class="form form--theme-xmas form--simple">
    <input class="form__text" type="text" />
    <input class="form__submit form__submit--disabled" type="submit" />
</form>
```

```css
.form { }
.form--theme-xmax { }
.form--simple { }
.form__text { }
.form__submit { }
.form__submit--disabled { }
```

- <a href="http://aleen42.github.io/" target="_blank" ><img src="./../pic/tail.gif"></a>