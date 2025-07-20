- Using the map() method in JavaScript to display data fetched from a third party or external provider differently in your app is a common use case of the map() method.
- The map() method in JavaScript is used to transform lists of data.
- When using the map() method, you will need to define a new variable, as it always returns a new array.
- When a JSX transformation will be part of the render method of components, you need to use curly braces to wrap your dynamic data so it can be accessed.
-  Amongst other things, keys instruct React on how to treat a specific element when updates happen.
-  Amongst other things, keys instruct React on whether a specific element’s internal state should be preserved when updates happen.
-  Keys are identifiers that help React determine which items have changed, are added or are removed.

# 1. What is "conditional rendering"?

It is a react method where any items/objects on the app/site render based on the given conditions

# 2. When would you use &&?

For conditional rendering when the value only depends on the first condition

# 3. When would you use a ternary?

When there are multiple conditions to justify the rendering of the elements

# 4. What if you need to decide between > 2 options on what to display?

ternary

# 5. In a vanilla JS app, at what point in the form submission process do you gather all the data from the filled-out form?
Right before the form is submitted.


# 6. In a React app, when do you gather all the data from the filled-out form?
As the form is being filled out. The data is all held in local state.


# 7. Which attribute in the form elements (value, name, onChange, etc.) should match the property name being held in state for that input?
`name` property.


# 8. What's different about saving the data from a checkbox element vs. other form elements?
A checkbox uses the `checked` property to determine what should
be saved in state. Other form elements use the `value` property instead.


# 9. How do you watch for a form submit? How can you trigger a form submit?
- Can watch for the submit with an onSubmit handler on the `form` element.
- Can trigger the form submit with a button click.

# 10. What are react's primary tasks?

- work with DOM/browser to render UI to the page

- Manage state for us between render cycles

- Keep the UI updated whenever state changes occur

# 11 What React can't handel on it's own?

- Outside effects
	- localStorage
	- API/database interactions
	- Subscriptions(ex: web sockets)
	- Syncing 2 different internal states together

# 12. What is a "side effect" in React? What are some examples?
- Any code that affects an outside system.
- local storage, API, websockets, two states to keep in sync


# 13. What is NOT a "side effect" in React? Examples?
- Anything that React is in charge of.
- Maintaining state, keeping the UI in sync with the data, 
  render DOM elements


# 14. When does React run your useEffect function? When does it NOT run the effect function?
- As soon as the component loads (first render)
- On every re-render of the component (assuming no dependencies array)
- Will NOT run the effect when the values of the dependencies in the
  array stay the same between renders


# 15. How would you explain what the "dependecies array" is?
- Second paramter to the useEffect function
- A way for React to know whether it should re-run the effect function

***Compound Components Quiz***

# 16. How would you explain the concept of compound components in React to someone who only knows the very basics of React?

- Components that work together to accomplish a greater objective than might make sense to try and accomplish with a single component alone.

# 17. What are some examples of HTML elements that work together to add functionality or styling to each other?


# 18. react.children

Children lets you manipulate and transform the JSX you received as the children prop.

```const mappedChildren = Children.map(children, child =>
  <div className="Row">
    {child}
  </div>
);
```

## Usage
- Transforming children
- Running some code for each child
- Counting children
- Converting children to an array

Children.map is similar to to transforming arrays with map(). The difference is that the children data structure is considered opaque. This means that even if it’s sometimes an array, you should not assume it’s an array or any other particular data type. This is why you should use Children.map if you need to transform it.

## Disadvantages
- fragile/delicate
- limited indepth


# 19. react.cloneElement()

cloneElement lets you create a new React element using another element as a starting point.

```const clonedElement = cloneElement(element, props, ...children)```

## Usage
Overriding props of an element

# 20. context

Usually, you will pass information from a parent component to a child component via props. But passing props can become verbose and inconvenient if you have to pass them through many components in the middle, or if many components in your app need the same information. Context lets the parent component make some information available to any component in the tree below it—no matter how deep—without passing it explicitly through props.

```import { createContext } from 'react';

export const LevelContext = createContext(1);
```

useContext is a Hook. Just like useState and useReducer, you can only call a Hook immediately inside a React component (not inside loops or conditions). useContext tells React that the Heading component wants to read the LevelContext.


## Use cases for context 
- *Theming:* If your app lets the user change its appearance (e.g. dark mode), you can put a context provider at the top of your app, and use that context in components that need to adjust their visual look.
- *Current account:* Many components might need to know the currently logged in user. Putting it in context makes it convenient to read it anywhere in the tree. Some apps also let you operate multiple accounts at the same time (e.g. to leave a comment as a different user). In those cases, it can be convenient to wrap a part of the UI into a nested provider with a different current account value.
- *Routing:* Most routing solutions use context internally to hold the current route. This is how every link “knows” whether it’s active or not. If you build your own router, you might want to do it too.
- *Managing state:* As your app grows, you might end up with a lot of state closer to the top of your app. Many distant components below may want to change it. It is common to use a reducer together with context to manage complex state and pass it down to distant components without too much hassle.
- ```<ul> & <li>, <select> & <option>, <table> & all the other table elements```

# 21. How can compound components help you avoid having to drill props multiple levels down?
   
- Compound component "flatten" the heirarchy that I would otherwise need to pass props through. Since I need to provide the children to render, the parent-most component has direct access to those "grandchild" components, to which it can pass whatever props it needs to pass directly.


# 22. compound components with dot syntax:

This is convenient if you have a single module that exports many React components. For example, if MyComponents.DatePicker is a component, you can use it directly from JSX with:

```
import React from 'react';

const MyComponents = {
  DatePicker: function DatePicker(props) {
    return <div>Imagine a {props.color} datepicker here.</div>;
  }
}

function BlueDatePicker() {
  return <MyComponents.DatePicker color="blue" />;
}
```

# 23. headless components

A Headless Component extracts all non-visual logic and state management, separating the brain of a component from its looks.

# 24. What is a route/url parameter?

A portion of our route path is a placeholder for what will eventually be the actual segment in the URL of the page.
