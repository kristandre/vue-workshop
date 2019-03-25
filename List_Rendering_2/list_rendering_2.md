# List Rendering 2
You can also access the properties of an object when iterating through an array with v-for.
```html
<ul>
  <li v-for="person in people">
    {{ person.firstName }}  {{ person.lastName }}
  </li>
</ul>
```

```javascript
data: {
  people: [
    {
      firstName: 'John',
      lastName: 'Doe'
    },
    {
      firstName: 'Jane',
      lastName: 'Doe'
    },
}
```

Result:
- John Doe
- Jane Doe

## Task
[Starting Code](https://jsfiddle.net/agv4dhzt/10/)

1. Add a list of variants to the data object:
```javascript
variants: [
    {
      id: 1,
      color: "brown",
      image: "https://bit.ly/2UN53VL"
    },
    {
      id: 2,
      color: "black",
      image: "https://bit.ly/2RXxsXC"
    },
    {
      id: 3,
      color: "red",
      image: "https://bit.ly/2HOWAO1"
    },
    {
      id: 4,
      color: "green",
      image: "https://bit.ly/2UYDKHW"
    }
  ],
```
2.Display the variant colors in a list below the details.

Next: [Event Handling](https://github.com/kristandre/vue-workshop/blob/master/Event_Handling/event_handling.md)

Previous: [List Rendering](https://github.com/kristandre/vue-workshop/blob/master/List_Rendering/list_rendering.md)

