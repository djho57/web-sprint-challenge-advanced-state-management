# Interview Answers
Be prepared to demonstrate your understanding of this week's concepts by answering questions on the following topics. These will not be counted as a part of your sprint score but will be helpful for preparing you for your endorsement interview, and enhancing overall understanding.

1. What problem does the context API help solve?
Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree. It helps keep code clean.

2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?
Actions- packets of information that contain an action type and associated data. Actions are objects that are passed to the reducer function as an argument, letting the reducer know how to update state.
Reducers- take two arguments, current state and action, and returns a new, updated state based on those arguments. Helps to manage changes in state without overriding initialState while also maintaining immutability.
Store- and object tree that contains the global state of the application. There is only one place to look to find the state of the app: the store.

3. What does `redux-thunk` allow us to do? How does it change our `action-creators`?
Makes the flow asynchronous and allows us to make API calls from action creators.

4. What is your favorite state management system you've learned and this sprint? Please explain why!
Redux-thunk, although confusing, was interesting to me because it allows us to integrate making API calls. It seems practical to be able to communicate with the API by making the action creators asynchronous. I believe once I'm able to make better sense of thunk it'll be very useful.