## :scope [**Back**](./../pseudoClass.md)

- The `:scope` CSS pseudo-class selector represents any element that is a `:scope` element.
- A **scope element** is an element that forms a context for a block of styles. Such an element also provides a reference point for selectors to match against.
- A scope element can be defined using the scoped attribute. A simple example would look like the following:

```html
<section>
    <style scoped>
        /* style declarations here apply to the <section>'s content */
        p {
            color: #0099cc; /* a blue color */
        }
    </style>
    <p>
        I am in the scope.
    </p>
</section>
<p>
    I am outside the scope.
</p>
```
- The styles declared inside a **style** element with a **scoped** attributes will be applied to any elements inside its parent element (the **section** in this example). These styles will also override the global styles defined in the document head (whether inline or via external style sheets).
- The `:scope` pseudo-class selector matches the context of the block of scoped styles. In the above example, the section element is matched by `:scope`. So, this:

```html
<section>
    <style scoped>
        /* style declarations here apply to the <section>'s content */
        p {
            color: #0099cc; /* a blue color */
        }
        
        :scope {
            background-color: #000;
        }
    </style>
    <p>
        I am in the scope.
    </p>
</section>
<p>
    I am outside the scope.
</p>
```

- Will apply a black background color to the section element. It is called the **scoping root** or the **local context** of `<style scoped>`.

<a href="http://aleen42.github.io/" target="_blank" ><img src="./../../../pic/tail.gif"></a>