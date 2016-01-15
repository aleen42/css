## Psedu-class [**Back**](./../types.md)

- When accessing a primitive type, you should work directly on its value.
    - `string`
    - `number`
    - `bool`
    - `null`
    - `undefined`

```js
const foo = 1;
let bar = foo;          /** number type */

bar = 9;

console.log(foo, bar);  /** => 1, 9     */
```

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../pic/tail.gif"></a>