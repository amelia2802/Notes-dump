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


# 9. How do you watch for a form submit? How can you trigger
   a form submit?
- Can watch for the submit with an onSubmit handler on the `form` element.
- Can trigger the form submit with a button click.
