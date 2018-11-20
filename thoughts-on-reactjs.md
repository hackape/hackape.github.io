# Thoughts on React.js

ref: https://medium.freecodecamp.org/is-mvc-dead-for-the-frontend-35b4d1fe39ec

React bring two very powerful idea to the table.

1. view as (pure) function of state
2. component-based architecture

But stateful component API is messy, it brings back one of the most evil thing in JSland back, the `this` context object.

## Make View PURE Again!

```jsx
// view.js

function HelloWorldView(state) {
  return <h1>{state.greeting}</h1>;
}
```

If view is guaranteed to be pure, we can build a lot of awesome stuff on top of it.

What about GUI interface building app to generate view code and styles? Enable UI/UX designers to production ready UI code.
