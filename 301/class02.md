# [State and Props](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)
What are component lifecycle events?
React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.


Mounting, Updating, and Unmounting are the three phases of the component lifecycle.
Mounting
When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.
Updating
Anytime a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order.
static getDerivedStateFromProps, shouldComponentUpdate, render,
getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps
Unmounting
The final phase of the lifecycle if called when a component is being removed from the DOM. componentWillUnmount is the only lifecycle event during this phase.
constructor()
The constructor for a React component is called before it is mounted.If the component is a subclass you should call super(props), or the props will be undefined. constructors can be used to assign state using this.state or to bind event handle methods to an instance. Let’s take a look at some example code.

UNSAFE Lifecycle Events
UNSAFE_componentWillMount()
UNSAFE_componentWillUpdate()
UNSAFE_componentWillReceiveProps()
These events have lead to a lot of bugs and unintended side effects, so in React 17 these will no longer be able to be used without the UNSAFE tag in front of them. Instead of componentWillMount use ComponentDidMount.
Instead of componentWillReceiveProps use static getDerivedStateFromProps.
Instead of componentWillUpdate us getSnapshotBeforeUpdate


## React Lifecycle Events
    - defined components as classes or functions
    - methods with the ability to be used are called lifecycle events
    - methods can be called during lifecycles of components
    - allow you to update UI / application states.
1. Based off the diagram, what happens first, the 'render' or the 'componentDidMount'?
    - It states that 'This method is invoked immediately after a component is mounted.
    - According to the diagram 'render' happens before 'componentDidMount'
2. What is the very first thing to happen in the lifecycle of React?
    - Mounting is the first phase of the component lifecycle of react.
3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
    - constructor, render, React Updates, componentDidMount, componentWillUnmount
4 .What does componentDidMount do?
    - It will load anything using a network request / initialize the DOM immediately after a component is mounted.
| Method | Side Effects 1 | State Updates | Example Uses |
| ------ | -------------- | ------------- | ------------ |
|Render | | | Create and Return Element(s)|
|ComponentDidMount| X | X | DOM Manipulations, network requests, etc.|
|Static getDerivedStatefromProps| | X | Update state based on changed props|
|shouldComponentUpdate| | X | Compare inputs and determine if render needed|
|getSnapshotBeforeUpdate| | | Set/reset things before next render|
|componentDidUpdate| X | X | DOM manipulations, network requests, etc. |
|componentWillUnmount| X | | DOM manipulations, network requests, etc. |
### notes cited from - (https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)
## React State vs Props
### Props
    - Similar to arguments to a function
    - Properties
1. What types of things can you pass in the props?
    - Things you want to render
    - Counters
    - Displays of titles of sub-titles
    - Displays information
2. What is the big difference between props and state?
    -States are handled inside of the component while props are handled outside of and passed into the component
    -States can be updated inside of the component props must be udpated outside.
3. When do we re-render our application?
    - When the states is changed inside of the application
4. What are some examples of things that we could store in state?
    - Incrimentation or Decrimentation
    - Items in which need to be updated





