
# [ Putting it all together]

## [React Docs - thinking in React](https://reactjs.org/docs/thinking-in-react.html)

React is, in our opinion, the premier way to build big, fast Web apps with JavaScript. It has scaled very well for us at Facebook and Instagram.

One of the many great parts of React is how it makes you think about apps as you build them. In this document, we’ll walk you through the thought process of building a searchable product data table using React.



1. How would you break a mock into a component heirarchy?

The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names. If you’re working with a designer, they may have already done this, so go talk to them! Their Photoshop layer names may end up being the names of your React components!

But how do you know what should be its own component? Use the same techniques for deciding if you should create a new function or object. One such technique is the single responsibility principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.


2. What is the single responsibility principle and how does it apply to components?

The single responsibility principle which means that a component is required to have only one reason to change. In short it means that the code with the same functionality should not exist in multiple places.


3. What does it mean to build a ‘static’ version of your application?

To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props. props are a way of passing data from parent to child. If you’re familiar with the concept of state, don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.


4. Once you have a static application, what do you need to add?

Step 1: Add Your New Site. …
Step 2: Link to Your GitHub (or supported version-control tool of choice) …
Step 3: Authorize Netlify. …
Step 4: Select Your Repo. …
Step 5: Configure Your Settings. …
Step 6: Build Your Site. …
Step 7: All Done.


5. What are the three questions you can ask to determine if something is state?
is the app in static version ? Is the app in interactivity ? Data is changed over time ?


6. How can you identify where state needs to live?
we need to identify which component mutates, or owns, this state.