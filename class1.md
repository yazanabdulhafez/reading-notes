# Introduction to React and Components

## Component Based Architecture

### Component

![component](https://rubygarage.s3.amazonaws.com/uploads/article_image/file/575/component-based-architecture.jpg)

React components are independent and reusable code. They are the building blocks of any React application. Components serve the same purpose as JavaScript functions, but work individually to return JSX code as elements for our UI.
Components usually come in the following types:

1. Functional Components: In simple words, Functional components are javascript functions.
2. Class Components.
3. Higher-Order Components.
4. Dumb Components.
5. Smart Components.
6. Presentational Components.
7. Container components.

### The charactistics of a component

1. Reusability − Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.

2. Replaceable − Components may be freely substituted with other similar components.

3. Not context specific − Components are designed to operate in different environments and contexts.

4. Extensible − A component can be extended from existing components to provide new behavior.

5. Encapsulated − A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.

6. Independent − Components are designed to have minimal dependencies on other components.

### The advantages of using component based architecture

1. Ease of deployment.

2. Reduced cost.

3. Ease of development.

4. Reusable.

5. Modification of technical complexity.

6. Reliability.

7. System maintenance and evolution.

8. Independent.

## What is Props and How to Use it in React

### What is props short for?

**Props**stands for properties. It is a special keyword in React which is used for passing data from one component to another.
Logically, components are just like JavaScript functions. They accept random inputs (called “props”) and return React elements which tell what should be displayed on the screen.

Props can be used to pass any kind of data such as:  

* String
* Array
* Integer
* Boolean
* Objects or,Functions

### How are props used in React

1. Firstly, define an attribute and its value(data)
2. Then pass it to child component(s) by using Props
3. Finally, render the Props Data

### The flow of props

Props have a one way downward binding between the parent and child component.
When the parent property updates, then the updates are passed into the child via props.
This prevents child components from accidentally mutating the parent’s state.

## Things I want to know more about

1. connecting the components with each other to build interface.
2. how to use the props inside a react app.

## Resources used in this read

1. <https://rubygarage.org/blog/the-angular-2-vs-react-contest-only-livens-up>
2. <https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm>
3. <https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0>
4. <https://blog.devgenius.io/vue-3-props-data-flow-2a03840a4197>
