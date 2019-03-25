# Event Handling
We can use the v-on directive to listen to DOM events and run some JavaScript when they’re triggered.

```html
<div id="app">
  <button v-on:click="counter += 1">Add 1</button>
  <p>The button above has been clicked {{ counter }} times.</p>
</div>
```
```javascript
var app = new Vue({
  el: '#app',
  data: {
    counter: 0
  }
})
```

### Methods
The logic for many event handlers will be more complex though, so keeping your JavaScript in the value of the v-on attribute isn’t feasible. That’s why v-on can also accept the name of a method you’d like to call.

```html
<div id="app">
  <button v-on:click="greet">Greet</button>
</div>
```
```javascript
var app = new Vue({
  el: '#app',
  data: {
    name: 'Vue.js'
  },
  // define methods under the `methods` object
  methods: {
    greet: function () {
      // `this` inside methods points to the Vue instance
      alert('Hello ' + this.name + '!')
    }
  }
})
```
Clicking the button will display the alert:
```
Hello Vue.js!
```
## Task
[Starting Code](https://jsfiddle.net/agv4dhzt/11/)

1. Add data property `{cartCount: 0}`
2. Create a button below the product variants, `Add to cart`.
3. Add a click event to the button that increments the `cartCount` decrement the `inventory` when it is clicked.
4. If the inventory is 0, disable the button.
5. Display the cartCount on the top of the page.

Next: [Event Handling 2](https://github.com/kristandre/vue-workshop/blob/master/Event_Handling_2/event_handling_2.md)

Previous: [List Rendering 2](https://github.com/kristandre/vue-workshop/blob/master/List_Rendering_2/list_rendering_2.md)

