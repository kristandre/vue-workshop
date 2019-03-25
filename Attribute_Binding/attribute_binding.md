# Attribute Binding

When we talk about data binding in Vue, we mean that the place where it is used or displayed in the template is directly linked, or bound to the source of the data, which is the data object inside the Vue instance.

```html
<div id="app">
  <a v-bind:href="url">Click me!</a>
  {{ message }}
</div>
```

```javascript
var app = new Vue({
  el: '#app',
  data: {
    url: 'https://google.com'
  }
})
```

## Task
[Starting Code](https://jsfiddle.net/agv4dhzt/7/)

1. Add an imageUrl property to the data object, `{imageUrl: 'https://bit.ly/2UN53VL'}`
2. Use attribute-binding in order to display an image above the `<h1>` header. Use the `imageUrl` as src.
3. Attach the product name as alt text to the image based on values from the instance’s data.

Next: [Conditional Rendering](https://github.com/kristandre/vue-workshop/blob/master/Conditional_Rendering/conditional_rendering.md)

Previous: [Vue Instance](https://github.com/kristandre/vue-workshop/blob/master/Vue_Instance/vue_instance.md)
