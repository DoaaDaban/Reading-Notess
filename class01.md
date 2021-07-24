# Component Based Architecture

## What is a component?

A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.

A component is a software object, intended to interact with other components, encapsulating certain functionality or a set of functionalities. It has an obviously defined interface and conforms to a recommended behavior common to all components within an architecture.

A software component can be defined as a unit of composition with a contractually specified interface and explicit context dependencies only. That is, a software component can be deployed independently and is subject to composition by third parties.

Views of a Component: 
1- Object-oriented view
2- Object-oriented view
3- Process-related view

## What are the charactistics of a component?

1- Reusability
2- Replaceable
3- Not context specific
4- Extensible
5- Encapsulated
6- Independent

## What are the advantages of using component based architecture?

Ease of deployment − As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.

Reduced cost − The use of third-party components allows you to spread the cost of development and maintenance.

Ease of development − Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.

Reusable − The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.

Modification of technical complexity − A component modifies the complexity through the use of a component container and its services.

Reliability − The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.

System maintenance and evolution − Easy to change and update the implementation without affecting the rest of the system.

Independent − Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

# What is Props and How to Use it in React

React is a component-based library which divides the UI into little reusable pieces. In some cases, those components need to communicate (send data to each other) and the way to pass data between components is by using props.
“Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another.
But the important part here is that data with props are being passed in a uni-directional flow. (one way from parent to child)
Furthermore, props data is read-only, which means that data coming from the parent should not be changed by child components.

I will be explaining how to use Props step by step.
Firstly, define an attribute and its value(data)
Then pass it to child component(s) by using Props
Finally, render the Props Data

## What is props short for?


“Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another. But the important part here is that data with props are being passed in a uni-directional flow

Props stand for properties and is a special keyword in React
Props are being passed to components like function arguments
Props can only be passed to components in one-way (parent to child)
Props data is immutable (read-only)

## How are props used in React?

Props are like parameters to a function  
Props cannot be changed, they are immutable  
A prop is a special keyword in React, that stands for properties  
Props can only be passed in a uni-direction i.e (parent to child)  
Props can be used to pass dynamic data to a component 
A component re-renders when data in the props change


## What is the flow of props?

 Flow is a static type checker for your JavaScript code. It is developed at Facebook and is often used with React. It lets you annotate the variables, functions, and React components with a special type syntax, and catch mistakes early.