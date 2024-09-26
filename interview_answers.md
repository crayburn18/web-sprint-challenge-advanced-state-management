# Interview Answers
Be prepared to demonstrate your understanding of this week's concepts by answering questions on the following topics. These will not be counted as a part of your sprint score but will be helpful for preparing you for your endorsement interview, and enhancing overall understanding.

1. What problem does the context API help solve?

Context API allows you to select the props from any level of the application without having to pass the prop all the way down through each level.

2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

Actions deliver an object from the component to the reducer.

 Reducers are a function that generate new state.  It uses a switch statement in order to know how to update the state. The data used to generate a new state comes from a payload recieved from the Action.

 Store is an immutable center for our components. Each component can access the store and select what state it needs. If other components want to change the state they must use actions.

3. What does `redux-thunk` allow us to do? How does it change our `action-creators`?

Redux-thunk is middleware intercepts the action before it gets to the reducer allowing it to be manipulated. Thunk allows us to make asynchronous actions.   

4. What is your favorite state management system you've learned and this sprint? Please explain why!

For a smaller application useState seems fine to me.  For larger applications I would choose Context API, as prop drilling starts to become impractical.