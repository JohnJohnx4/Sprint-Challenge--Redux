1. Name 3 JavaScript Array/Object Methods that do not produce side-effects? Which method do we use to create a new object while extending the properties of another object?
array.map, array.slice, Object.assign
Object.assign(...object, props, etc)

2. Describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

actions - dispatch a "action type" to a reducer based on what the action is doing, and is used to get, store, or update data.

reducers - return the changed state without mutating the original state based on the action type

store - is what stores the state and cannot be changed witout dispatching an action. It is the single source of truth because it holds all the information on the state, and all other pieces need store to function.

3. What is the difference between Application state and Component state? When would be a good time to use one over the other?

Application state is held within store and component state is held within the class of that component. Application state is better for when the whole application needs the updated state, and component state is better for just updating specific components and the whole application doesnt need updating.

4. What is middleware?

middleware provides a third-party extension point between dispatching an action and the moment it hits a reducer. 

5. Describe `redux-thunk`, what does it allow us to do? How does it change our `action-creators`?

thunk allows redux to recognize functions as actions and allows async

6. Which `react-redux` method links up our `components` with our `redux store`?

Connect lines up components with the store