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

# 4. What if you need to decide between > 2 options on
   what to display?

ternary

# 5. In a vanilla JS app, at what point in the form submission
   process do you gather all the data from the filled-out form?
Right before the form is submitted.


# 6. In a React app, when do you gather all the data from
   the filled-out form?
As the form is being filled out. The data is all held in local state.


# 7. Which attribute in the form elements (value, name, onChange, etc.)
   should match the property name being held in state for that input?
`name` property.


# 8. What's different about saving the data from a checkbox element
   vs. other form elements?
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


# 14. When does React run your useEffect function? When does it NOT run
   the effect function?
- As soon as the component loads (first render)
- On every re-render of the component (assuming no dependencies array)
- Will NOT run the effect when the values of the dependencies in the
  array stay the same between renders


# 15. How would you explain what the "dependecies array" is?
- Second paramter to the useEffect function
- A way for React to know whether it should re-run the effect function

