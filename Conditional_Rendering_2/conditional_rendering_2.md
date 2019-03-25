# Conditional Rendering 2

The v-else-if, as the name suggests, serves as an “else if block” for v-if. It can also be chained multiple times:
```html
<div v-if="type === 'A'">
  A
</div>
<div v-else-if="type === 'B'">
  B
</div>
<div v-else-if="type === 'C'">
  C
</div>
<div v-else>
  Not A/B/C
</div>
```
## Task
[Starting Code](https://jsfiddle.net/agv4dhzt/8/)

1. Replace the `inStock` data property with an inventory property, `{inventory: 5}`
2. In the `<p>` element below the `<h1>` header display `In stock!` if the inventory is greater than 10.
3. Display `Almost empty!` if inventory is between 1 and 10.
3. Display `Not in stock` if inventory is 0.

Next: [List Rendering](https://github.com/kristandre/vue-workshop/blob/master/List_Rendering/list_rendering.md)

Previous: [Conditional Rendering](https://github.com/kristandre/vue-workshop/blob/master/Conditional_Rendering/conditional_rendering.md)

