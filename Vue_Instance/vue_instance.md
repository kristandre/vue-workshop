# Vue instance

A Vue instance is the root of our application. It is created by passing an options object into it. Just like it sounds, this object has a variety of optional properties that give the instance the ability to store data and perform actions.

```javascript
var app = new Vue({
  // options
})
```

When a Vue instance is created, it adds all the properties found in its data object to Vue’s reactivity system. When the values of those properties change, the view will “react”, updating to match the new values.

```html
<div id="app">
  {{ message }}
</div>
```

```javascript
var app = new Vue({
  el: '#app',
  data: {
    message: 'Hello Vue!'
  }
})
```

```
Hello Vue!
```

## Task
[Starting Code](https://jsfiddle.net/agv4dhzt/3/)

1. Create a new Vue instance, and bind it to the `<div id="app">` element.
2. Create a data object inside the Vue instance.
3. Create a new property in the data object, `productName: 'shoes'`.
4. Render `productName` inside an `<h1>` tag in the template.

Next: [Attribute Binding](https://github.com/kristandre/vue-workshop/blob/master/Attribute_Binding/attribute_binding.md)
