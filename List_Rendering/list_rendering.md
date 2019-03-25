# List Rendering
We can use the v-for directive to render a list of items based on an array. The v-for directive requires a special syntax in the form of item in items, where items is the source data array and item is an alias for the array element being iterated on:
```html
<ul id="app">
  <li v-for="item in items">
    {{ item.message }}
  </li>
</ul>
```

```javascript
var app = new Vue({
  el: '#app',
  data: {
    items: [
      { message: 'Foo' },
      { message: 'Bar' }
    ]
  }
})
```

Result:
- Foo
- Bar

## Task
[Starting Code](https://jsfiddle.net/agv4dhzt/9/)

1. Add a list of details to the data object, `details: ["Leather", "Waterproof"],`.
2. Display the details in a list below the inventory status.

Next: [List Rendering 2](https://github.com/kristandre/vue-workshop/blob/master/List_Rendering_2/list_rendering_2.md)

Previous: [Conditional Rendering 2](https://github.com/kristandre/vue-workshop/blob/master/Conditional_Rendering_2/conditional_rendering_2.md)

