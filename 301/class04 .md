 # [React and Forms](https://reactjs.org/docs/forms.html)


1. What is a ‘Controlled Component’?

A Controlled Component is one that takes its current value through props and notifies changes through callbacks like onChange. A parent component "controls" it by handling the callback and managing its own state and passing the new values as props to the controlled component. You could also call this a "dumb component".
A Uncontrolled Component is one that stores its own state internally, and you query the DOM using a ref to find its current value when you need it. This is a bit more like traditional HTML.


2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

it depends to the usage of the form.

3. How do we target what the user is entering if we have an event handler on an input field?

 target the input value using the event object and pass it to method to either change the state or to use it for any other purpose.


# [The Conditional (Ternary) Operator Explained](https://reactjs.org/docs/conditional-rendering.html)

- Why would we use a ternary operator?
The Ternary operator is a shorter and easier way to write a conditional statement in Javascript.


Rewrite the following statement using a ternary statement:

``` js

  if(x===y){
 console.log(true);
  } else {
 console.log(false);

 ```
We can rewrite the following conditional statement using the Ternary operator : <

``` js
x === y ? console.log(true) : console.log(false);

```

 # [React Bootstrap - Forms](https://react-bootstrap.github.io/components/forms/)

# [React Docs - conditional rendering](https://reactjs.org/docs/conditional-rendering.html)