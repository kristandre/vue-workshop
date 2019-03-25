# Conditional Rendering

The directive v-if is used to conditionally render a block. The block will only be rendered if the directive’s expression returns a truthy value.
```html
<h1 v-if="awesome">Vue is awesome!</h1>
```
It is also possible to add an “else block” with v-else:
```html
<h1 v-if="awesome">Vue is awesome!</h1>
<h1 v-else>Oh no 😢</h1>
```
## Task
[Starting Code](https://jsfiddle.net/agv4dhzt/5/)

1. Create a new data property, `{inStock: true}`
2. Create a `<p>` element below the `<h1>` header.
3. Inside `<p>` display `In stock!` if the product is in stock.
3. Display `Not in stock` if the product is not in stock.

Next: [Conditional Rendering 2](https://github.com/kristandre/vue-workshop/blob/master/Conditional_Rendering_2/conditional_rendering_2.md)

Previous: [Attribute Binding](https://github.com/kristandre/vue-workshop/blob/master/Attribute_Binding/attribute_binding.md)

